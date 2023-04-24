## 1. What is MongoDB?
- MongoDb  is a opensource Nosql database 
- it stores the data in flexible json -like documents with dynamic schemas
## 2. What are the benefits of using MongoDB?
- Flexible data Model : Mongo is flexible document model  it ca store the data as it fits to application needs
- Scalability 
- High availability: it provides the automatic failover and replication make sure that data is always available even if hardware fails
- Performance : mongo is document model and index based make it fast quering and reteriving the data
- Rich query language
- OpenSource and community -driven
- Integration with tools
## 3. What is the difference between MongoDB and SQL databases?
- Data Model : 
```
sql  database use a rigid, table-based datamodel with fixed schemas
Mongodb database use a flexible document-based data model with dynamic schemas 
```
- Querying language : 
```
Sql follows the sql query language primaryly 
mongo db follows the json-based query language
```
- Scalability : 
```
sql database traditionally scale up , as data grows  it goes to single server
mongodb scale out ,as data distrub multiple server
```
- Acid compliance : sql database typically follow acid properties , mongo db provides less strict consistency guarantees 
## 4. What is a document in MongoDB?
- A Document is a data structure that contains a set of key-value pairs
- it is basic unit to store data 
- it represents the single entity or record in collection
- Documents contains nested structures,arrays and other data types
## 5. What is a collection in MongoDB?
- a collection is a group of related documents that are stored together in the database.
- Each document in a collection can have a different structure or schema, which means that collections are schema-less.
- db.createCollection("users");
## 6. What is the use of the ObjectId in MongoDB?
- The ObjectId is a unique identifier that MongoDB uses to identify each document in a collection.
-  It is a 12-byte binary value that consists of a timestamp, a machine identifier, a process identifier, and a random counter value.
- object id is automatically generated when ever document is created
- it used to retrive the data easily
## 7. What is the use of the $set operator in MongoDB?
- $set operator is used to update operator to update the fields in the document if that field doesn't exists it creates the field
- it takes field name and its value
- set is used to update multiple fields
## 8. What is the use of the $push operator in MongoDB?
- $push operator is a update operator used for add elements to an array in mongodb
- it takes two values field name and value 
- if that field name doesn't exists it create new array with the field if it already exists and it is not array it returns an error 
- we can also add multiple elements by providing the array
## 9. What is the use of the $pull operator in MongoDB?
- $pull is a update operator used to remove all instance of a specified value  from a array field
## 10. What is the use of the $inc operator in MongoDB?
- $inc is a update operator used to increment the value of a numeric field
```
db.collection.updateOne(
{ _id: ObjectId("6155b1848d85539d5c5c03b2") },
{ $inc: { stock: 5 } }
)

```
## 11. What is the use of the $gte operator in MongoDB?
- the $gte operator in MongoDB is a useful comparison operator that allows you to select documents where the value of a specified field is greater than or equal to a specified value.
```
db.orders.find({ total: { $gte: 100 } })

```
## 12. What is the use of the $and operator in MongoDB?
- $and is a logical operator used to combine the multiple conditions as a single query using the AND operator
````
db.collection.find({ $and: [ { <condition1> }, { <condition2> }, ... ] })

````
## 13. What is the use of the $or operator in MongoDB?
- $or is a logical operator used to combine the multiple conditions as a single query using the OR operator
```
db.products.find({ $or: [ { category: "electronics" }, { name: /smart/ } ] })

```
## 14. What is the use of the $regex operator in MongoDB?
- $regex operator is a query operator that allows you to search for documents based on a specified regular expression pattern
```
db.books.find({ title: { $regex: /python/ } })

```
## 15. What is the use of the $in operator in MongoDB?
- $in is a query operator used to find documents where the value of a field matches with any of the values specified in an array.
```
db.customers.find({ state: { $in: ["California", "Texas", "New York"] } })

```
## 16. What is sharding in MongoDB?
- sharding is a method in mongo for distributing data across the multiple servers or machines
- sharding is a technique used in MongoDB to horizontally scale a database by distributing data across multiple servers or machines. It provides several benefits, including horizontal scalability, high availability, better performance, and cost-effectiveness.
## 17. What is replication in MongoDB?
- Replication in MongoDB is the process of synchronizing data across multiple servers
- MongoDB replication creates multiple copies of data and distributes it across different servers, also known as replica sets, so that if one server fails, another server can take over and continue serving data.
- replication in MongoDB is the process of synchronizing data across multiple servers to ensure high availability, fault tolerance, and better read scalability. It is a key feature of MongoDB that provides reliability and performance for modern applications.
## 18. What is the use of the aggregation pipeline in MongoDB?
- The aggregation pipeline is a powerful feature of MongoDB that allows you to perform complex data processing and analysis operations on your collections. By using the aggregation pipeline, you can reduce the amount of data that needs to be transferred between your application and the database, and you can perform data processing operations directly in the database, which can improve performance and scalability.
## 19. What is indexing in MongoDB?
- 
## 20. What is the use of the text index in MongoDB?

