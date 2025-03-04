#### Start mongoDB service

- net start mongoDB

#### Stop mongoDB service

- net stop MongoDB

#### Use mongoDB

- mongo

#### List Databases

- show dbs

#### Switch Databases

- use [databaseName]

#### Current database

- db

#### Create a collection

db.createCollection("[collectionName]")

#### List all collections

- db.getCollectionNames()
- show collections

#### Insert a document

- db.[collectionName].insert({ [key]: "[value]" })

#### Query all documents

- db.[collectionName].find()

#### Delete a single document

- db.[collectionName].deleteOne({ [key]: "[value]" });

#### Empty a MongoDB collection

- db.[collectionName].deleteMany({});

#### Drop a collection

- db.[collectionName].drop()

#### View database statistics

- db.stats()

#### View server status

- db.serverStatus()
