# E-Commerce-Back-End
AS A manager at an internet retail company
I WANT a back end for my e-commerce website that uses the latest technologies
SO THAT my company can compete with other e-commerce companies

GIVEN a functional Express.js API
WHEN I add my database name, MySQL username, and MySQL password to an environment variable file
THEN I am able to connect to a database using Sequelize
WHEN I enter schema and seed commands
THEN a development database is created and is seeded with test data
WHEN I enter the command to invoke the application
THEN my server is started and the Sequelize models are synced to the MySQL database
WHEN I open API GET routes in Insomnia Core for categories, products, or tags
THEN the data for each of these routes is displayed in a formatted JSON
WHEN I test API POST, PUT, and DELETE routes in Insomnia Core
THEN I am able to successfully create, update, and delete data in my database

## Installation
npm init to create package.json
npm i mysql2 package for mysql database
npm i sequelize package to connect to Express.js API
npm i dotenv to use enviroment variables to store sensitive data.
npm run seed to seed data to database
node server.js to run server
## Usage
Database models

*Category
id
Integer.
Doesn't allow null values.
Set as primary key.
Uses auto increment.


*category_name
String.
Doesn't allow null values.


*Product
id
Integer.
Doesn't allow null values.
Set as primary key.
Uses auto increment.


*product_name
String.
Doesn't allow null values.


*price
Decimal.
Doesn't allow null values.
Validates that the value is a decimal.


*stock
Integer.
Doesn't allow null values.
Set a default value of 10.
Validates that the value is numeric.


*category_id
Integer.
References the Category model's id.


*Tag
id
Integer.
Doesn't allow null values.
Set as primary key.
Uses auto increment.


*ProductTag
id
Integer.
Doesn't allow null values.
Set as primary key.
Uses auto increment.


*tag_name
String.


*product_id
Integer.
References the Product model's id.


*tag_id
Integer.
References the Tag model's id.


db folder that holds schema.sql file to create mysql database

