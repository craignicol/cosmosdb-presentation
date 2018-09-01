# Introduction to CosmosDb

## What is CosmosDb

* Microsoft blurb - globally scalable

---

## Global...

## Multi-engine...

## Configurable...

---

## In development...

Some use cases are production ready, with great documentation. Others less so.

---

## The APIs

* SQL (LINQ over JSON, fka DocumentDb)
* Table (Key-Value) - mostly compatible with Azure Table
* Graph API (using the Gremlin graph traversal language)
* MongoDb
* Cassandra

** NOTE : Think of DocumentDb as 1.0, CosmosDb as 2.0, but what you really want is 2.1 Not realy interested in MongoDb and Cassandra in this talk - think of it as IaaS for those APIs.

---

## Data structure (SQL API)

* It's not relational
* Don't try and join between documents, you can only join within to traverse hierarchy
* What queries do you need to optimise?
* It's no longer about 3NF
  * Remember the SQL API is SQL syntax on NoSql data

---

## Data structure (Table API)

* It's actually KV pair

---

## Data structure (Graph API)

* Nodes and vertices
* Models relationships (e.g. social media)
* Support Gremlin language for queries

---

## Indexing

* Index all the things
* ...but sometimes you need to tune

---

## Partitioning

* Automatically partition
* Choose a key that adequately distributed the data
* CosmosDb will automatically cluster

---

## JS in the database?

* Stored procs
* UDF
* Triggers
  * Azure Functions  

---

## New considerations

* RUs?
  * A measure of computational complexity. Can be hard to predict. So build, test, and measure. Pricing is based on allocating enough resources for x00 RUs.
* Tuneable consistency
  * (new slide with image on this)
  
---

## Local development

* CosmosDb emulator (and limitations)
  * Only SQL and Table API
  * Does not support any consistency model (so only single-threading for dev)
  * Does support UDF and SPs
  
---

## C# 

* Creating models
* LINQ and conventions
  * Silent failures 
* Automapping is very nice, when it works

---

## Example

Room booking system

* Number of sites
* Each site has multiple employees
* Each site has multiple rooms
* Each room can have multiple events
- OR -
* Events have their own collection
* Each event has a start and end time (fun with timezones)
* Each event has a title
* Each event has an attendee list
* Each event may have on-line details

---

## Conclusion

---

## Questions?
  
