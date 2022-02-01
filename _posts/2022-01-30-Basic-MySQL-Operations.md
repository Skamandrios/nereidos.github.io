---
layout: post
category: Linux Guides
---

# MySQL Operations and Commands

> Some mysql commands (still in progress...)


## Table of contents
- [SHOW and USE DB](#SHOW and USE DB)
- [Create database and tables](#Create database and tables)
- [Show content in Tables](#Show content in Tables)
- [Insert into Table](#Insert into Table)
- [Update Table](#Update Table)
- [ADD COLUMN](#ADD COLUMN)
- [Search in Table](#Search in Table)

## [SHOW and USE DB](#SHOW and USE DB)
- Show all databases

```
 SHOW DATABASES;
```

- use database

```
 use testdb;
```
- show all tables

```
 show tables;
```

## [Create database and tables](#Create database and tables)
- create database

```
 create database testdb;
```

- Create table named Users

``` 
 CREATE TABLE Users ( Username varchar(255), Firstname varchar(255),Lastname varchar(255) Age int, Country varchar(255), Active BOOLEAN );
```

- Create tabel with ID with an auto-increment

```
 CREATE TABLE Users2 (ID INT AUTO_INCREMENT PRIMARY KEY, Username varchar(255), Firstname varchar(255),Lastname varchar(255), Age int, Country varchar(255), Active BOOLEAN );
```

## [Show content in Tables](#Show content in Tables)

- show content

```
 SELECT * FROM Users;
```

- show chracktertype

```
 desc Users;
```

## [Insert into Table](#Insert into Table)
- Insert to all

```
 INSERT INTO Users(Username,Active) VALUES('t');
 INSERT INTO Users(Username,Username) VALUES('max.muster');
 INSERT INTO Users(Username) VALUES('max.muster');
 INSERT INTO Users(Username) VALUES('max.muster');
 INSERT INTO Users(Firstname) VALUES('max');
 INSERT INTO Users(Firstname) VALUES('max');
```

- Insert into all columns

```
 INSERT INTO Users(Username,Firstname,Lastname,Age,Country,Active) VALUES('johnny.down','johnny','down','25','CH','t');
 INSERT INTO Users(Username,Firstname,Lastname,Age,Country,Active) VALUES('klaus.wolf','klaus','wolf','22','DE','t');
```

## [Update Table](#Update Table)

---
{: data-content="Elias"}