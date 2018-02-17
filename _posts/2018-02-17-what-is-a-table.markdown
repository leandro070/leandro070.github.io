---
title: "What is a table?"
layout: post
date: 2018-02-17 00:20:00
image: /assets/images/header_database_course.jpeg
headerImage: true
tag:
- database
- table
- exercise
star: true
category: blog
author: leandro070
description: What is, how work and how build a table.
---

The table is **the most important element** in a database, and it is fundamental you understand **what is it, how work it, and how build it**.

## What is it

>A table is a collection of related data held in a structured format within a database.

Well, let's take a moment and analyze the definition. **A table is a collection of related data**. To understand what a table is, we need be capable of abstracting the reality. 

If you are a owner of a cars dealership, probably you have many cars, and probably you have a cars stock. This stock is a table. There are many cars models in stock. And you need control what models car you have and how much cars you have.

This is a *collection of related data*, **a lot of data with similar features encompasses under a generic name**, "Cars", Cars is table title.

The database table is **where all the data** in a database is stored, and without tables, there would not be much use for relational databases.

## How work it

Every table consist of two structures:

**Column**: Each column contain same type data. For example: Names (String), Years(Integer), Dates(Date). A column is defined by its name and data type.

**Row**: A table can contain zero or more rows.  When there are zero, it said to be empty. Each row can represent an real object.

*Example:*

**Car table:**

| ID_CAR   | Brand  | Model | Year | HP   | Price |
| -------- | ------ | ----- | ---- | ---- | ----- |
| 00231242 | AUDI   | A1    | 2017 | 95   | 28000 |
| 00101134 | BMW    | 320   | 2015 | 180  | 25000 |
| 00450002 | Toyota | Camry | 2018 | 301  | 24400 |

**Every table have a ID column** or Primary Key (PK), this ID is unique, usually auto-incremental, and identify each row. In other chapter we learn more of this

## How build it

In other case, we need to store personal data of users.For example: Name, Last Name, Age, User Name, 
Password. 

Each data that we want to store of a person is a attribute. **An attribute represents an interest property of an entity**.

| ID_user| name | last_name | age | user_name   | password |
| -------- | ------ | ----- | ---- | ---- | ----- |
| 001 | Leandro  | Gutierrez  | 24 | leandro070  | 1234 |
| 002 | Will  | Papein | 18 | willpp  | asdfg |
| 003 | Linus | Torvalds | 48 | LinuxRules  | password1234 |

Later, we have the data that we want to store and the table attributes. We need to name the table in some way, we will look for an easy and descriptive name for the data in the table. I like "Users" because we have 'User Name' and 'Password'.

**Table Name: Users**

------

## Exercise!

**Now, your turn**. Try to make this exercise:

I have a market and I need to store all money receipts
* Find the table name
* Find attributes
*Remember,don't forget the ID attribute*

### Solution 

There are many solution, a possible solution is this:
![Markdowm Image][1]
![Markdowm Image][2]

**See you soon!**


[1]: /assets/images/what_is_a_table/table.png
[1]: /assets/images/what_is_a_table/table_gui.png
