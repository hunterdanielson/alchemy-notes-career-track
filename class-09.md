# Alchemy Reading Notes

## Class 09

### Mongoose Instance Methods
- Instances of Models are documents. Documents have many of their own built-in instance methods. We may also define our own custom document instance methods.
- Add custom instance method example 
  ```javascript
   // define a schema
  var animalSchema = new Schema({ name: String, type: String });

  // assign a function to the "methods" object of our animalSchema
  animalSchema.methods.findSimilarTypes = function(cb) {
    return mongoose.model('Animal').find({ type: this.type }, cb);
  };
  ```
  - Make sure not to overwrite default mongoose methods, can be unpredictable

### Mongoose Static Methods
- There are two equivalent ways to add a static:

1. Add a function property to schema.statics
1. Call the Schema#static() function
- Example
  ```javascript
  // Assign a function to the "statics" object of our animalSchema
  animalSchema.statics.findByName = function(name) {
    return this.find({ name: new RegExp(name, 'i') });
  };
  // Or, equivalently, you can call `animalSchema.static()`.
  animalSchema.static('findByBreed', function(breed) {
    return this.find({ breed });
  });

  const Animal = mongoose.model('Animal', animalSchema);
  let animals = await Animal.findByName('fido');
  animals = animals.concat(await Animal.findByBreed('Poodle'));
  ```
- **Don't** declare statics with **=>**, it prevents *this* binding

### Mongoose Middleware
- Middleware (also called pre and post hooks) are functions which are passed control during execution of asynchronous functions. Middleware is specified on the schema level.
