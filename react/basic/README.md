# React lolaDB Example

A basic example that shows how to use [lolaDB](https://loladb.com?utm_source=github&utm_medium=js-framework-examples&utm_campaign=react) with React

For these demos to work on your local machine as shown in the example, you must first complete the preqrequisites described below.

This example allows you to query any connected datbase, including MySQL, PostgreSQL, MariaDB, and more. See a full list of supported databases here: [lolaDB Supported Sources](https://docs.loladb.com/guides/supported-sources/?utm_source=github&utm_medium=js-framework-examples&utm_campaign=react)

## lolaDB Docs

You can always reference the [lolaDB Developer Docs](https://docs.loladb.com/?utm_source=github&utm_medium=js-framework-examples&utm_campaign=react) for more information.

## Available Scripts

```bash
# Install Dependencies
npm i
```

## Developing

```bash
# Run the app
npm start
```

## Prerequisites

### Test Data Setup

For this example to work on your local machine as shown in the examples, you must setup a database with an 'orders' table. The table should have the following columns:

- orderId
- productName
- quantity
- customerId

Insert some dummy data. You can use the following SQL statement:

```sql
INSERT INTO (orderId, productName, quantity, customerId) VALUES (3589491, 'KosmicKrush', 12, 384164);
INSERT INTO (orderId, productName, quantity, customerId) VALUES (3589488, 'MoonMist', 6, 897788);
INSERT INTO (orderId, productName, quantity, customerId) VALUES (3589490, 'CosmiGulp', 5, 794576);
INSERT INTO (orderId, productName, quantity, customerId) VALUES (3589489, 'Stardrizzle', 3, 637786);
INSERT INTO (orderId, productName, quantity, customerId) VALUES (3589495, 'AstroFizz', 13, 737786);
```

### Create your query

Within the lolaDB UI, create a `Source` within your `Hub` that connects to your database. Create a `Query` that selects the data you want to display in your frontend application. You can use the following SQL statement:

```sql

SELECT * FROM orders;

```

Save your query and copy the `Query ID` from the top right hand corner to use in your demo app.
