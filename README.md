<h1><center>Document, Ledger and Search Databases</center></h1>

<p align="center">
  <img src="https://community-cdn-digitalocean-com.global.ssl.fastly.net/assets/tutorials/images/large/Database-Mostov_v4.1_twitter-_-facebook.png?1546896970?raw=true" alt="Sublime's custom image"/>
</p>



## Preface
We recently had a video conference with a friend of our professor Juan vazquez named Paco Ocampo, Paco is a person who knows about managing the cloud for big data and this time he told us about the different types of databases that we can find in the google cloud.

Although databases are essential today for any public and private company, why? This is due to the fact that they are more efficient when storing information (without papers) and less contamination, but without a doubt one of their main advantages of using them is the great value that we can obtain from them, as we usually hear "When life hands you lemons, make lemonade. ", with the data we can even predict the future.

But if you want to know about databases you can search for pages, documents, books among other types of resources, that is why in this document we will focus on the different types of databases that currently exist, we hope you like it .


## Document databases

This type of database is built similar to a JSON file,
XML & YAML or binary formats such as BSON so if we have knowledge of this type of document either because we program in JavaScript or use them to build data frames in python with the help of pandas.

> Here is an example of what the format would look like:

![ejemplo1](https://webassets.mongodb.com/_com_assets/cms/Code%20Snippet%20545%20x%20330@4x-zgzlrug0va.png)


This type is one of the most popular alternatives that can be used as rational tabular databases and according to Wikipedia they constitute one of the main subcategories within the so-called NoSQL databases.

Some characteristics that we will talk about later are the following:

> Natural and flexible 

> They promise higher developer productivity, and faster evolution with application needs.

Here some examples of systems of Document Databases

![imagen3](https://www.practicalecommerce.com/wp-content/uploads/2016/07/070116-nosql-db-570x276.png)


# Different between relational databases

## Intuitive data model:
> The documents are assigned to the objects in the code, this makes it easier to work with them.

> As shown in the first image, the structure of this database is different from a DB SQL, therefore we will not need to execute "joins" that consume a lot of resources.

> We can put the data together or as pipes, this allows us to write less code and gives us more performance for queries.

## Flexible Scheme:
> The documents are dynamic, this means that it is not necessary to define them previously in the DB.

> The fields of the documents can vary, and the structures can be modified at the moment we want, allowing us to avoid disruptive schema migrations.

## Powerful:
> Ad hoc queries, indexing, and real-time aggregations provide powerful ways to access, transform, and analyze your data.

> With the help of ACID transactions, the same guarantees are maintained as a DB SQL, that is, we can manipulate data from a single document or multiple documents that live in multiple fragments.

## The Distribution:
> These databases are systems distributed at their core, so each document is independent of another, this provides us with an ease when it comes to distributing them on various servers.

> According to the document DB mongo dB page, native fragmentation provides an elastic and transparent horizontal scale to the application to accommodate the growth of its workload, along with geographic data distribution for data sovereignty.

# Graphical difference between a relational database and one based on documents

![imagen4](https://webassets.mongodb.com/_com_assets/cms/Relational_vs_DocumentDB-imgngssl17.png)


## Ledger Database.
### Why “ledger”?

The term ledger represents the way we used to record information before computers. Before computers, we recorded information in books, sometimes called ledgers, where data was only appended and you could view the past. In the early years of computers, hardware was expensive. Thus we built systems that update in place and use the most efficient amount of memory. Now that we’re in the age of cheap, commodity hardware, we can revert to recording information in a more intuitive and useful way.

*"Ledger Database — A NoSQL database that provides an immutable, transparent, and cryptographically verifiable transaction log •owned by a central authority. — Amazon’s QLDB Overview"*

*"A non ledger database is table-centric. A ledger database is log-centric. The log is the database."*

To begin with:
* it is not a NoSQL database (usually)
This is different from the usually NoSQL database we're getting, it's different form Microsoft SQL Server, Oracle, MYSQL servers.
Data is stored as a document without and natural relationships to other documents, but in this case this works as a relational database. 
* It is immutable.
In ledger databases, these can never been changed. So no matter what changes happen you will never overwrite the existing data. 
* It is trasnparent.
It's the ability to see the changes to records and data over time. 
* It is cryptographically verified.
This mean that the records or data are hashed. In a simple way the long string of data that is the record is paired down to a much smaller string of characters that is unique. 

### How does work it?
Let's suppose that we create an order:
![ex1](https://ivan.mw/images/ledger-1.jpg)
Then We update it.
![ex2](https://ivan.mw/images/ledger-2.jpg)
Then we do update it again
![ex3](https://ivan.mw/images/ledger-3.jpg)

The key insight is that ledger databases remember the past. New information doesn’t overwrite the past but is instead added to it. The log is the heart of the database and the source of truth, not the tables. Each update is appended to the log as a new entry.
### Example of legder based architecture
![ex4](https://ivan.mw/images/ledger-4.jpg)

The ledger database contains the log and tables which are a view into the log’s data. In this case, I have an Orders table which shows the latest status of each order. That same log data is fed into an email system, which emails customers updates on their orders, a billing system, which filters through log data and tracks each CREATED order, and a data warehouse, which is used to run analytics on the data.

## Flexible Scheme:


## Matrix 
| Criteria             |   |   |   |   |   |
|----------------------|---|---|---|---|---|
| Best used            |   |   |   |   |   |
| Usage example        |   |   |   |   |   |
| Known Shortcomings   |   |   |   |   |   |
| Main focus           |   |   |   |   |   |
| License              |   |   |   |   |   |
| Pricing              |   |   |   |   |   |
| Projects using it    |   |   |   |   |   |
| Latest version       |   |   |   |   |   |
| Data Presentation    |   |   |   |   |   |
| Development language |   |   |   |   |   |
| Platforms            |   |   |   |   |   |
| Website              |   |   |   |   |   |
|                      |   |   |   |   |   |
|                      |   |   |   |   |   |
|                      |   |   |   |   |   |


**References:**
* https://ivan.mw/2019-11-24/what-is-a-ledger-database
* https://hackernoon.com/relational-nosql-ledger-databases-work-not-permissioned-blockchains-9ccaef7b3139
* https://medium.com/a-technologists-pov/do-i-need-a-ledger-database-what-is-it-6f3b7261238


