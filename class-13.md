# Alchemy Reading Notes

## Class 13

### Aggregation Pipeline
The aggregation pipeline is a framework for data aggregation modeled on the concept of data processing pipelines. Documents enter a multi-stage pipeline that transforms the documents into aggregated results.

Getting an aggregation pipeline started is a simple affair: simply call the aggregate function on any collection.

- Example
```javascript
{
  "id": "1",
  "firstName": "Jane",
  "lastName": "Doe",
  "phoneNumber": "555-555-1212",
  "city": "Beverly Hills",
  "state: "CA",
  "zip": 90210
  "email": "Jane.Doe@compose.io"
}
```
- To begin an aggregation on the customers collection, we call the aggregate function on the customers collection:
```javascript
> db.customers.aggregate([ ... aggregation steps go here ...]);
```

- To match it is like a SQL WHERE clause or a MongoDB find, example:
```javascript
> db.customers.aggregate([ 
  { $match: { "zip": 90210 }}
]);
```

- Can then group them into subsets, example:
```javascript
> db.customers.aggregate([ 
  { $match: {"zip": "90210"}}, 
  { 
    $group: {
      _id: null, 
      count: {
        $sum: 1
      }
    }
  }
]);
```
