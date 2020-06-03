# Alchemy Reading Notes
## Class 03


1. Why would a developer choose to make data models?
    - Data modeling is the act of exploring data-oriented structures. Like other modeling artifacts data models can be used for a variety of purposes, from high-level conceptual models. Practically speaking it is helpful to have an idea of the shape of the data for the whole team for whole team understanding.
1. What purpose do CRUD operations serve?
    - In computer programming, create, read, update, and delete (CRUD) are the four basic functions of persistent storage.
1. What kind of database is Postgres? What kind of database is MongoDB?
    - PostgreSQL is a general purpose and object-relational database management system, the most advanced open source database system.
    - MongoDB is a cross-platform document-oriented database program. Classified as a NoSQL database program, MongoDB uses JSON-like documents with optional schemas.
1. What is Mongoose and why do we need it?
    - Mongoose provides a straight-forward, schema-based solution to model your application data. It includes built-in type casting, validation, query building, business logic hooks and more, out of the box. In simple words, Mongoose acts as an intermediate between mongodb and server side language(like NodeJs) [Source](https://www.quora.com/What-is-Mongoose)
1. Define three related pieces of data in a possible application. An example for a store application might be Product, Category and Department. Describe the constraints and rules on each piece of data and how you would relate these pieces to each other. For example, each Product has a Category and belongs in a Department.
    - Pokemon: Type, ID, Stats
    - Each Pokemon would have an ID specific to it, has a type or two, and it also has stats associated with the specific Pokemon

| Term | Definition |
| ------------- |:-------------:|
| database | A structured set of data held in a computer, especially one that is accessible in various ways. |
| data model | A data model (or datamodel) is an abstract model that organizes elements of data and standardizes how they relate to one another and to the properties of real-world entities. |
| CRUD | Create, Read, Update, Delete |
| schema | A schema (pronounced SKEE-mah) is the organization or structure for a database. |
| sanitize | Sanitizing will remove any illegal character from the data. |
| Structured Query Language (SQL) | Structured Query Language. SQL is used to communicate with a database. |
| Non SQL (NoSQL) | A NoSQL database provides a mechanism for storage and retrieval of data that is modeled in means other than the tabular relations used in relational databases. |
| MongoDB | MongoDB is a cross-platform document-oriented database program. Classified as a NoSQL database program. |
| Mongoose | Mongoose provides a straight-forward, schema-based solution to model your application data. |
| record | Record (computer science) In computer science, a record (also called a structure, struct, or compound data) is a basic data structure. |
| document | Any written text, illustrations or video that describe a software or program to its users is called program or software document. |
| Object Relation Mapping (ORM) | A programming technique for converting data between incompatible type systems using object-oriented programming languages. This creates, in effect, a "virtual object database" that can be used from within the programming language. |