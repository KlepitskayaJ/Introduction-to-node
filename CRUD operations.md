Sure, here's a brief summary in English on the topic of CRUD operations using Mongoose methods:

CRUD stands for Create, Read, Update, and Delete. These are the fundamental operations that can be performed on data in a database. 

Here are some examples of how you might use Mongoose methods for each operation:

```javascript
// Create
let newDocument = new Model({ /* your data here */ });
newDocument.save(function (err) {
  if (err) return handleError(err);
  // saved!
});

// Read
Model.find({ /* your query here */ }, function (err, docs) {
  if (err) return handleError(err);
  // docs contains the documents that match the query
});

// Update
Model.updateOne({ /* your query here */ }, { /* your update here */ }, function(err, res) {
  if (err) return handleError(err);
  // res.nModified contains the number of documents updated
});

// Delete
Model.deleteOne({ /* your query here */ }, function (err) {
  if (err) return handleError(err);
  // deleted
});
```

Remember to replace `Model` with your actual model, and replace the comments with your actual data, query, or update. Also, make sure to handle errors appropriately in your actual code. These are just basic examples and might need to be adjusted based on your specific use case. 

I hope this helps! Let me know if you have any other questions.
