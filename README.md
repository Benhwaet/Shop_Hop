# Shop_Hop

Your One Stop Shop - Only a Web Hop Away

## Description

Bounce into this back-end for an e-commerce site. It uses nodejs, an express.js API to use Sequelize to interact with a MySQL database, and dotenv to store sensitive data like the database password.
The purpose of this project is to familiarize myself with these technologies and understand the fundamental structure of a back-end for an e-commerce site.

The User Story and Acceptance Criteria, provided by edX (see credits), are as follows:

### User Story

```md
AS A manager at an internet retail company
I WANT a back end for my e-commerce website that uses the latest technologies
SO THAT my company can compete with other e-commerce companies
```

### Acceptance Criteria

```md
GIVEN a functional Express.js API
WHEN I add my database name, MySQL username, and MySQL password to an environment variable file
THEN I am able to connect to a database using Sequelize
WHEN I enter schema and seed commands
THEN a development database is created and is seeded with test data
WHEN I enter the command to invoke the application
THEN my server is started and the Sequelize models are synced to the MySQL database
WHEN I open API GET routes in Insomnia for categories, products, or tags
THEN the data for each of these routes is displayed in a formatted JSON
WHEN I test API POST, PUT, and DELETE routes in Insomnia
THEN I am able to successfully create, update, and delete data in my database
```

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [Credits](#credits)
- [License](#license)

## Installation

1. Clone the repo
2. Install NPM packages

   ```sh
   npm install
   ```

3. Create a .env file in the root directory and add the following:

   ```sh
    DB_NAME='ecommerce_db'
    DB_USER='root'
    DB_PASSWORD='your password'
    ```

--> The following steps are shown in the video that follows them.
4. Run the schema.sql file in the db folder in MySQL Workbench OR run the following in the terminal:

   ```sh
   mysql -u root -p
   ```

then,

   ```sh
   source db/schema.sql
   ```

5. Seed the database by running the following in the terminal:

   ```sh
    npm run seed
    ```

See this [video](https://drive.google.com/file/d/1YySAl7om3KIDmSAr25970vNB4Klz1SCY/view?usp=sharing) to see the steps above and the first step in Usage below.

## Usage

In order to run the application, run the following in the terminal:

```sh
npm start
```

OR

```sh
node server.js
```

The API will then be active and can be tested in Insomnia Core, as shown in this video:

[ShopHop API Demo](https://drive.google.com/file/d/1ThSKlH85t3wWta2zwFpqjHltN1yboUNJ/view?usp=sharing)

## Credits

The starter code for this project was provided by edX in the scope of a Full-Stack Development Bootcamp hosted by the University of New Brunswick.
The code is heavily based on the module for Object-Relational Mapping (ORM) with Sequelize, module 13, or the course.

## License

The MIT License is used in this project. See the LICENSE file for details.
