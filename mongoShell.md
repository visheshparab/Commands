#### Start mongoDB service

- Win: net start mongoDB

#### Stop mongoDB service

- Win: net stop MongoDB

#### Use mongoDB

- Win: mongo

#### List Databases

- Win: show dbs

#### Switch Databases

- Win: use [databaseName]

#### Current database

- Win: db

#### Create a collection

db.createCollection("[collectionName]")

#### Insert a document

- Win: db.[collectionName].insert({ [key]: "[value]" })

#### Query all documents

- Win: db.[collectionName].find()

#### Drop a collection

- Win: db.[collectionName].drop()

#### View database statistics

- Win: db.stats()

#### View server status

- Win: db.serverStatus()
