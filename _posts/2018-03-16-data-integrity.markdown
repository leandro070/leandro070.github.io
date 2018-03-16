---
title: "Data Integrity"
layout: post
date: 2018-03-16 12:30:00
image: /assets/images/header_database_course.jpeg
headerImage: true
tag:
- database
- table
- domain
star: true
category: blog
author: leandro070
description: Integrity ensures that the data in a database is both accurate and complete, in other words, that the data makes sense.
---

Integrity ensures that the data in a database is both accurate and complete, in other words, that the data makes sense. 

## Key Constraints

A relation is defined as a set of tuples. There can not be two tuples that have the same
combination of values for all its attributes.

The UNIQUE constraint ensures that all values in a column are different.

Another constraints on the attributes that  you specify  if you allows or not NULL values.

In general, a relational scheme may have more of a key. In this case, each one of them they call Candidate Key. 

Is habitual appoint one of the Candidate Key as Primary Key of the relation. This key has a UNIQUE constraint and cannot contain NULL values.

A Foreign Key is other Candidate Key and is a key used to link two tables together. This is a field (or collection of fields) in one table that refers to the Primary Key in another table. The table containing the foreign key is called the child table, and the table containing the candidate key is called the referenced or parent table. Foreign Key may be NULL or duplicate 

## Entity Integrity

Entity Integrity ensures that there are no duplicate records within the table and that the field that identifies each record within the table is unique and never null. 

The existence of the PRIMARY KEY is the core of the entity integrity. If you define a primary key for each entity, they follow the entity integrity rule.

## Domain Constraints

A domain is defined as the set of all unique values permitted for an attribute.  For example, a domain of date is the set of all possible valid dates, a domain of integer is all possible whole numbers, a domain of day-of-week is Monday, Tuesday ... Sunday.

This in effect is defining rules for a particular attribute.  If it is determined that an attribute is a date then it should be implemented in the database to prevent invalid dates being entered.

If the system supports domain constraints then this invalid data 
would not have stored in the first place.  That is, the integrity of the
 database is being preserved.

**SQL EXAMPLE**

For example I want to create a table “student_info” with “stu_id” field having value greater than 100, I can create a domain and table like this:

```sql
create domain id_value int
constraint id_test
check(value > 100);

create table student_info (
stu_id id_value PRIMARY KEY,
stu_name varchar(30),
stu_age int
);
```


