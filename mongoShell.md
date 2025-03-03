#### Start mongoDB service

- Win: net start mongoDB

#### Stop mongoDB service

- Win: net stop MongoDB

#### Use mongoDB

- Win: mongo
- mac: mongosh "mongodb+srv://cluster0.r5dwp.mongodb.net/" --apiVersion 1 --username visheshparab

#### List Databases

- show dbs

#### Switch Databases

- use [databaseName]

#### Current database

- db

#### Create a collection

   - db.createCollection("[collectionName]")

#### List all collections

- db.getCollectionNames()
- show collections

#### Insert a document

- db.[collectionName].insert({ [key]: [value] })        (insert document)
- db.[collectionName].insertOne({ [key]: [value] })     (for one document)
- db.[collectionName].insertMany({ [key]: [value] })    (for many documents)

#### Find all documents

- db.[collectionName].find()

#### Find required document with exact search value
   - db.[collectionName].find({ [key]: [value] })

#### Find required document with conditional search value (&& condition)
   - db.[collectionName].find({ [key]: {$lte: [value]}, [key]: {$gte: [value]} })    ($lte - less then equal, $gte - greater than equal)

#### Find required document with conditional search value (|| condition)
   - db.[collectionName].find({ $or: [ { [key]: { $lte: [value] }}, { [key]: { $gte: [value] }}]})   ($or - OR operator)

#### Find required document only with specific key field in result
   - db.[collectionName].find({},{ [key]: 1 })
   - db.[collectionName].find({ [key]: {$lte: [value]}}, { [key]: 1 })

#### Update query (you can also set new key)
   - db.[collectionName].updateOne({ [key]: [value] }, { $set: { [key]: [value]}})
   - db.[collectionName].updateMany({ [key]: [value] }, { $set: { [key]: [value]}})

#### Replace query (same as update only difference it does not contain $set operator and replaceMany)
   - db.[collectionName].replaceOne({ [key]: { $gte: [value] }, rating: { $gte: 4.8 } }, { [key]: [value], rating: 4.8, premium: false })

#### Delete query
   - db.[collectionName].deleteOne({ [key]: [value]})
   - db.[collectionName].deleteMany({ [key]: {$lte: [value]}})
   - db.[collectionName].deleteMany({})

#### Drop a collection

- db.[collectionName].drop()

#### View database statistics

- db.stats()

#### View server status

- db.serverStatus()

#### Quit mongoDB shell
   - quit()
