# Mongo Aggregation Pipeline
https://docs.mongodb.com/manual/core/aggregation-pipeline/

* First Stage: The $match stage filters the documents by the status field and passes to the next stage those documents that have status equal to "A".

* Second Stage: The $group stage groups the documents by the cust_id field to calculate the sum of the amount for each unique cust_id.

* each stage transforms the documents as they pass through the pipeline

* some pipeline stages take pipeline expressions as the operand

# Aggregations in MongoDB by Example
https://www.compose.com/articles/aggregations-in-mongodb-by-example/

* aggregate function accepts an array of data transformations which are applied to the data in the order they're defined

* first stage is Matching Documents
  -only takes what you want to work with 
* second is grouping documents
  -groups into subsets based on what you want to do with that data
* third is transactions
  -can sum, min, max, avg
