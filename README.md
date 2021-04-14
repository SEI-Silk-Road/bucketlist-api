# Bucket List - Back end 

Keep track of your life's dreams

Part 1 of 2. As a back end application it makes use of Mongoose, MongoDB, Express, Node.js, Javascript, and cors, among other middleware to tell our app how to communicate with the server 

(Schema)

(Router)

## Table of Contents

* [General Info](#general-info)
* [Technologies](#technologies)
* [Hosted]
* [Diagrams](#diagrams)
* [User Stories](#user-stories)
* [Unsolved Problems](#unsolved-problems)
* [Images](#images)

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
* Passport 0.4.1
* Node 10.15.0
* NPM 6.4.1

## Hosted @ Heroku
<br />

## Diagrams

<br />

## User Stories

## Unsolved Problems

## Images


This application allows the user create a list of the things they have always wants to do and cross them off as they achieve their goals. We wanted to create this application because it was both something we want to use ourselves and because it was something relatively simple that would allow us to create an immersive, seamless user experience.

## Important Links

-   [Other Repo](https://github.com/SEI-Silk-Road/bucketlist-client)
-   [Deployed API](https://gentle-journey-02010.herokuapp.com/)
-   [Deployed Client](https://sei-silk-road.github.io/bucketlist-client/)

## Planning Story

Our journey began in a discussion assigning roles to the members of our group with
Aidan Kenney, the Project and Back-end Lead, Huy Ngyuen, Front-end Lead, and
Bryan Braunstein, the Quality Assurance Lead. This encouraged us to stay
organized since the moment we started and we really starting planning to attack
our schema the way that would make the most sense to the extencity of our
project and also to our skill level. We knew it would not be too difficult, to
have one list with many items and this would allow us to focus on some reach goals
once we could successfully interact with all of our endpoints in the process to
CRUD a resource. We finished this without to much effort, besides figuring out
how to update the state of a currently rendered page and then dived right into
some fun additions such as *Unsplash* background and a pagination feature.
Overall, we got to really get hands on with two new interesting roles in software,
building in React and working with version control amongst a team!

### User Stories

-   As a user I want to sign in/up
-   As a user I want to Create a new resource
-   As a user I want to Read multiple resources
-   As a user I want to Read a single resource
-   As a user I want to Update a resource I own
-   As a user I want to Delete a resource I own

### Technologies Used

-   Mongoose
-   MongoDB
-   CORS
-   Javascript
-   Express

### Unsolved Problems

-   Still need to add more options for movability around the app.
-   Would like to eventually integrate a Google Maps API with a place search so
that users can pin on a map where they would like to carry out their bucketlist
items.

## Images

* * *

#### ERD: <https://imgur.com/a/A4dJlCB>

### Authentication

| Verb   | URI Pattern            | Controller#Action |
|--------|------------------------|-------------------|
| POST   | `/sign-up`             | `users#signup`    |
| POST   | `/sign-in`             | `users#signin`    |
| PATCH  | `/change-password/`    | `users#changepw`  |
| DELETE | `/sign-out/`           | `users#signout`   |

### Event Management

| Verb   | URI Pattern             | Controller#Action   |
|--------|-------------------------|---------------------|
| GET    | `/items`                | `items#index`       |
| GET    | `/items/:id`            | `items#show`        |
| POST   | `/items`                | `items#create`      |
| PATCH  | `/items/:id`            | `items#update`      |
| DELETE | `/items/:id`            | `items#delete`      |
