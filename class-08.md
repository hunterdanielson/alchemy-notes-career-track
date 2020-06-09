# Alchemy Reading Notes

## Class 08

### Mongoose Populate
- lets you reference documents in other collections
- links together different schemas
- can connect them via the _id value
- populated() lets you check if there is a value, returns truthy if there is
- depopulate() lets you remove a populated value

### Express Router
What exactly is the Express Router? It is a mini express application without all the bells and whistles of an express application, just the routing stuff

Route middleware in Express is a way to do something before a request is processed. This could be things like checking if a user is authenticated, logging data for analytics, or anything else we'd like to do before we actually spit out information to our user.

**The order you place your middleware and routes is very important** Everything will happen in the order that they appear

### Mongoose Virtuals
Basically lets you populate on other things than the _id value