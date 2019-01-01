# Stateful and Stateless: Serverless apps with Redis

## Elevator Pitch (300 characters)
Function-as-a-Service (FaaS) platforms enable developers to deploy code, get a network endpoint that invokes it, and never maintain the underlying infrastructure of pay for idle time. Serverless functions enables quick iterations and fast development. They also introduce new design patterns and best practices. As these functions are short-lived and distributed, they can not hold the state of the system. Traditional ACID DBMS solutions might not handle hundreds of concurrent connections efficiently.

Enter Redis!

In this session I will build a live CRUD app on stage using serverless functions and Redis. In every development step, I will explain the design choices and design patterns being used. The app will be available on github, and developers will be able to deploy it in 5 minutes after the session is over. Developers attending this session will gain basic understanding of Serverless design patterns and best practices, and practical tools for deploying a low-latency app backed by a Redis instance.
If internet connection allows, the audience will be able to interact with the app using their cellphones.

## Technical level
* Redis knowledge is assumed.
* No prior Serverless knowledge assumed.

## Talk Format
Short session (20 minutes).

## Special requirements
* WiFi / Cellular reception
* Projector podium

## Outline
* Basic Serverless concepts: Functions, design patterns, stateless architecture, some best practices (5-7 minutes)
* Building a CRUD app function from 3 function (5-7 minutes)
* Audience interaction with the app using cell phones (3 minutes)
* Q&A / Spare time (3 minutes)