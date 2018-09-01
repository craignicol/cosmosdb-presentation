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
* Table (Key-Value)
* MongoDb
* Cassandra
* Gremlin
* Graph API

** NOTE : Think of DocumentDb as 1.0, CosmosDb as 2.0, but what you really want is 2.1

---

## Data structure (SQL API)

* It's not relational
* Don't try and join between documents, you can only join within to traverse hierarchy
* What queries do you need to optimise?

---

## Data structure (Table API)

* It's actually KV pair

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
* Scalable consistency

---

## Local development

* CosmosDb emulator (and limitations)

---

## C#

* Creating models
* LINQ and conventions
  * Silent failures 

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
  
