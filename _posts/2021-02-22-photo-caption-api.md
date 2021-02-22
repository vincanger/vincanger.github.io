---
title: "Photo Caption API"
date: 2021-02-22
tags: [Passport, ExpressJS, Redis, Sequelize]
excerpt: "Local Authentication with Passport, Redis caching, Sequelize ORM"
---
see the code on [GitHub](https://github.com/vincanger/photo-caption-api)

## Description

This is an API that allows the client/users to add captions to photos.
The server runs on ExpressJS, Passport for local authentication, Redis to cache user sessions, and Sequelize as the ORM to communicate with a Postgres database.

### Preview

<img src="https://github.com/vincanger/photo-caption-api/blob/master/photo-app-preview.gif?raw=true" />

### Objective

This was a learning project. My goals were to learn and implement:

1. Sequelize ORM ✅
2. Local Passport authentication ✅
3. User sessions with Express/Passport ✅
4. Redis ✅
5. Configure Redis, Sequelize, and Postgres for successful deployment to Heroku ✅
    - https://photo-caption.herokuapp.com 🧙‍♂️
