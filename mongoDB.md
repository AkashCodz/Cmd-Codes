# MongoDB Cheat Sheet

## Download MongoDB

## Connect to MongoDB Shell
- `mongo`: Connect to local MongoDB instance.
- `mongo "mongodb://192.168.1.1:27017"`: Connect to MongoDB instance on a local network.
- By default, connects to `mongodb://127.0.0.1:27017`.

## Connect to MongoDB Atlas
- `mongo "mongodbURI" --username <username>`: Connect to MongoDB Atlas instance.

## Database Operations
- `show dbs`: Show all databases.
- `db`: Show current database.
- `use client`: Create or switch to a new database.
- `db.dropDatabase()`: Delete the current database.

## Collections
- `show collections`: Show all collections in the current database.
- `db.createCollection('courses')`: Create a new collection named 'courses'.

## Create Documents
- `db.courses.insertOne({...})`: Insert one document into the 'courses' collection.
- `db.courses.insert({...})`: Insert one or more documents into the 'courses' collection.
- `db.courses.insert({...}, {...})`: Insert multiple documents into the 'courses' collection.

## Read Documents
- `db.courses.findOne()`: Find one document in the 'courses' collection.
- `db.courses.find()`: Find multiple documents in the 'courses' collection.
- `db.courses.find().pretty()`: Find multiple documents in the 'courses' collection and display them in a formatted way.
- `db.courses.find({...})`: Find documents in the 'courses' collection based on specified criteria.

## Update Documents
- `db.courses.updateOne({...}, {...})`: Update one document in the 'courses' collection.
- `db.courses.update({...}, {...})`: Update multiple documents in the 'courses' collection.
- `db.courses.update({...}, {...})`: Update sub-documents in the 'courses' collection.

## Delete Documents
- `db.courses.remove({...})`: Delete documents from the 'courses' collection.

## Count
- `db.courses.find().count()`: Count the number of documents in the 'courses' collection.

## Sorting
- `db.courses.find().sort({...})`: Sort documents in the 'courses' collection.

## Pagination
- `db.courses.find().skip(n)`: Skip n results in the 'courses' collection.
- `db.courses.find().limit(n)`: Limit the number of results returned in the 'courses' collection.

## Indexing
- `db.courses.createIndex({...})`: Create indexes on fields in the 'courses' collection.
- `db.courses.dropIndex({...})`: Drop indexes from the 'courses' collection.

## Text Search
- `db.courses.createIndex({"name": "text"})`: Create a text index on the 'name' field for text search.
- `db.courses.find({$content: {$search: "JS"}})`: Search documents in the 'courses' collection by text.

## Range Query
- `db.courses.find({"views": {'$gt': 70}})`: Find documents where 'views' are greater than 70.
- `db.courses.find({"views": {'$gte': 70}})`: Find documents where 'views' are greater than or equal to 70.
- `db.courses.find({"views": {'$lt': 70}})`: Find documents where 'views' are less than 70.
- `db.courses.find({"views": {'$lte': 70}})`: Find documents where 'views' are less than or equal to 70.

