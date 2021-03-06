- First Stage: The $match stage filters the documents by the status field and passes to the next stage those documents that have status equal to "A".
- Second Stage: The $group stage groups the documents by the cust_id field to calculate the sum of the amount for each unique cust_id.
- Some pipeline stages take a pipeline expression as the operand. Pipeline expressions specify the transformation to apply to the input documents. Expressions have a document structure and can contain other expression.
- The aggregate function accepts an array of data transformations which are applied to the data in the order they're defined. 
- The first stage of the pipeline is matching, and that allows us to filter out documents so that we're only manipulating the documents we care about.
- The $gte and $lt operators are comparators that allow us to limit our dates to specific range.
