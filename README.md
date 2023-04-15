## Book Now API

Learning project to learn cloud computing and typescript as a private side project.

This app is a Serverless REST api for buying E-books using Azure Functions and CosmosDB with TypeScript.

**Table of Contents**

[TOCM]

[TOC]

----

## Roadmap

This project is in an initial stage and is intented to be completed over the course of 2 weeks.
The following are the features that will be completed first:

1. Connect Azure functions with database in azure
2. Populate database with mock data
3. Write integration test for main features using jest
   1. View superagent package in npm
   2. View how to mock database using local storage
4. Make `GET /api/books` endpoint avaliable through the web
5. Include auth features
   1. View azure-middleware
   2. Search for oauth2 auth and JWT in azure functions
6. Rewrite README.md with following steps

---

## Technologies used

|  Tecnology  |  Version |
| ------------ | ------------ |
| Typescript  | 4.9.5  |
|  Azure Functions  |  4.0.4915  |
| CosmosDB | NA |
|  Jest  |  29.4.3  |

----

## API Reference

#### GET /api/books - List all available books.

```PowerShell
curl -i [insert url]
```

#### POST /api/books/buy/{id} - Buy a ebook.

```PowerShell
curl -X POST -i [insert url] -d {[isert data]}
```

Param | Type | Description
:--- | :--- | :---:
`id` | Integer | true

#### GET /api/categories/{category} - List all available books of an specific category.
```PowerShell
curl -i [insert url]
```

#### GET /api/categories - List all categories.

```PowerShell
curl -i [insert url]
```

#### GET /api/users - Obtain current user info.

```PowerShell
curl -i [insert url]
```

#### POST /api/users/signup - Register new user.

```PowerShell
curl -i [insert url]
```

#### POST /api/users/auth - Obtain access JWT token.

```PowerShell
curl -i [insert url]
```

----

## Author

- [Alberto Ortiz](https://github.com/tizor98)


### Sequence Diagram

-Base code for make a diagram at the end of the project

```seq
Client->Server: Says Hello 
Note right of Server: Server thinks\nabout it 
Server-->Client: How are you? 
Client->>Server: I am good thanks!
```

## End