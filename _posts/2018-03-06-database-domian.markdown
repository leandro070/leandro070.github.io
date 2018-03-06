---
title: "Database Domain"
layout: post
date: 2018-03-06 13:00:00
image: /assets/images/header_database_course.jpeg
headerImage: true
tag:
- database
- table
- domain
star: true
category: blog
author: leandro070
description: The domains make a powerful feature of relational model.
---

The domains **make a powerful feature** of relational model. A domain describes a set of possible values for a certain attribute. Each database attribute is defined over a domain, and could be many attributes defined above the same domain. 

| Attribute | Domain | Description | Definition|
| ---- |---- | ---- | ---- |
|carID | car_id_dom | Car dentification code | 8 digit number|
| branch | car_branch_dom | Car branch | 30 characters |
| model | car_model_dom | Car model, it isn't the manufacture year| 30 characters |
| year | car_year_dom | the manufacture year | 4 digit number|

**The domain concept is important** because it allows the user define the meaning and the values that  attributes can take. In this way, there are more available information for the system when this one going to execute a relational operation. 

Different types of domains are: integers, strings, date, non-procedural, etc.
As a domain restricts the values of the attribute, it can be considered as a restriction.

## SQL Example:
**CREATE DOMAIN** POSITIVE **AS** INTEGER NOT NULL CHECK(VALUE > 0);

**CREATE TABLE** countryside(
id: integer not null primary key,
hectares: positive);

Information extracted from:
*Base de datos - Mercedes Marqués*
*https://ignorante.wordpress.com/2007/06/04/dominios-sql/*
