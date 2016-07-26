# dynamodb-milkhatx

Limitations:
* Does not work with DynamoDBMapper. Users need to build their own marshalling.
* Low-level data model is constrained by the immutability assumption.
* No support for lock stealing. Transactions have to wait for previous transactions to complete or be swept.

Advantages:
* Supports LSIs, GSIs, Scans and Queries.
* Consumes less DynamoDB resources.
* Transactions are low-latency; 10s of milliseconds.
