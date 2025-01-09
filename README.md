# Incorrect MongoDB Aggregation Pipeline

This repository demonstrates a common error in MongoDB aggregation pipelines where an improperly placed `$match` stage can lead to inaccurate results in the `$group` stage. 

The `bug.js` file contains code that shows an aggregation pipeline with a potential issue, causing the `$group` stage to not accurately count documents after the `$match` filter.

The `bugSolution.js` file provides a corrected version, demonstrating how to correctly order aggregation stages to avoid such issues.

## How to reproduce the bug

1. Clone this repository.
2. Run the `bug.js` script using a MongoDB shell.
3. Observe the result of the aggregation and compare it to the expected results (see detailed explanation in bugSolution.js).

## How to solve the bug

Review the corrected pipeline in `bugSolution.js` to see how to structure an aggregation pipeline to correctly handle filtering and grouping operations.