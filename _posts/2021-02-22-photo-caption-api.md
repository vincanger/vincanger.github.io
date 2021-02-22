---
title: "Photo Caption API"
date: 2021-01-19
tags: [Passport, ExpressJS, Redis, Sequelize]
excerpt: "Local Authentication with Passport, Redis caching, Sequelize ORM"
---
see the code on [GitHub](https://github.com/vincanger/photo-caption-api)

## Description

This is an API that allows the client/users to add captions to photos. 
The server runs on ExpressJS, Passport for local authentication, REDIS to cache user sessions, and Sequelize as the ORM to communicate with a Postgres database

### Preview

<img src="https://github.com/vincanger/photo-caption-api/blob/master/photo-app-preview.gif?raw=true" />

### Objective

This was a learning project. My goals were to learn and implement:

1. Sequelize ORM :white_check_mark:
2. Local Passport authentication :white_check_mark:
3. User sessions with Express/Passport :white_check_mark:
4. Redis :white_check_mark:
5. Configure Redis, Sequelize, and Postgres for successful deployment to Heroku :white_check_mark:
    - https://photo-caption.herokuapp.com :thumbsup:
