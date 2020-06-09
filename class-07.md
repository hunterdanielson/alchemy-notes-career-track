# Alchemy Reading Notes

## Class 07

### Express Routing
- Event driven system
    - ```javascript
        app.get('/thing', (req,res) => {})
        ```

### The Request Object
-   ```javascript
    (req,..)
    /:parameters
    app.get('/api/:thing',...) = req.   params.thing
    ```
### Query Strings
- ```javascript 
    http://server/route?ball=round = req.query.ball
    ```

### Response Object

- ```javascript
    (...,res)
    ```
- Other methods like send() and status()

### Middleware
- A series of functions the request goes through
- Each function has a request, response, and next
- Types of middleware: 
    - Application
    - Route
### CRUD Operations
```javascript
CREATE
app.post('/resource')
READ
app.get('/resource')
UPDATE
app.put('/resource/:id')
DESTROY
app.get('/resource/:id')
```

### Server Testing
- Generally avoid testing on actual server
- Use supertest, as it is a separate instance of the server



