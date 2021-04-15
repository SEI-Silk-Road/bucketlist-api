# Bucket List - Back End 

Keep track of your life's dreams!

### [Visit Live Site](https://sei-silk-road.github.io/bucketlist-client/) / [Front End Code](https://github.com/SEI-Silk-Road/bucketlist-client) / [Heroku](https://gentle-journey-02010.herokuapp.com/)


## Table of Contents

* [General Info](#general-info)
* [Technologies](#technologies)
* [Schemas](#schemas)
* [User Stories](#user-stories)
* [Unsolved Problems](#unsolved-problems)
* [Images](#images)
* [Authentication](#authentication)
* [Event Management](#event-management)
* [Our Team](#our-team)

## General Info 

Used Javascript, Express to make an API, Mongoose to create a schema, and MongoDB as our database.

## Technologies 

Project is created with: 

* Javascript
* Mongoose 5.8.1
* MongoDB 3.4.0
* Express 4.17.1
* JSONWebToken 8.5.1
* Bcrypt 3.0.7
* CORS 2.8.5
* Passport 0.4.1
* Node 10.15.0
* NPM 6.4.1

## Schemas 
*In Mongoose we start with a Schema. Each schema maps to a MongoDB collection and defines the shape of the documents within that collection.*

<img src="https://i.imgur.com/caR9EgJ.jpg" alt="MongoDB structure">

### Collections:

__Item Schema__ 
<img src="https://i.imgur.com/VjztBjj.png" alt="item schema">

Shown here is our item schema where the key value pairs make up our documents.

__User Schema__
<img src="https://i.imgur.com/dh9iaDm.png" alt="user schema">

And here our actual user schema.
<br />

## User Stories
-   As a user I want to sign in/up
-   As a user I want to Create a new resource
-   As a user I want to Read multiple resources
-   As a user I want to Read a single resource
-   As a user I want to Update a resource I own
-   As a user I want to Delete a resource I own
## Unsolved Problems
* Could use work in the UI department
* Integrate Google Maps API

## Images
### [ERD](https://imgur.com/a/A4dJlCB)
<br />

## Authentication

| Verb   | URI Pattern            | Controller#Action |
|--------|------------------------|-------------------|
| POST   | `/sign-up`             | `users#signup`    |
| POST   | `/sign-in`             | `users#signin`    |
| PATCH  | `/change-password/`    | `users#changepw`  |
| DELETE | `/sign-out/`           | `users#signout`   |
<br />

## Event Management
Using the express.Router class in the ***routes.js*** files, we're able to handle all of our client requests in one modular file.

| Verb   | URI Pattern             | Controller#Action   |
|--------|-------------------------|---------------------|
| GET    | `/items`                | `items#index`       |
| GET    | `/items/:id`            | `items#show`        |
| POST   | `/items`                | `items#create`      |
| PATCH  | `/items/:id`            | `items#update`      |
| DELETE | `/items/:id`            | `items#delete`      |
<br />

## Our Team

Bryan Braunstein, the Project and Quality Assurance Lead, Huy Ngyuen, Front-end Lead, and Aidan Kenney, the Back-end Lead.

Scrum/Agile