# JSHunt

[![npm version](https://badge.fury.io/js/node.svg)](https://badge.fury.io/js/node)

## Description

A simple Node.js backend application created in the [Skylab](https://skylab.rocketseat.com.br) Starter Node.js course by [RocketSeat](https://rocketseat.com.br/). This app handles data from a MongoDB database with ***mongoose*** and uses ***express*** to provide an api to front-end clients.

## Installation

1. Install [node.js](https://nodejs.org/en/)
2. Run `git clone https://github.com/luisfelipesantos/jshunt-backend.git`
3. Go into the cloned folder. `cd jshunt-backend`
4. Run `npm install`
5. Run `npm start`

The app uses a MongoDB database. So you must have a MongoDB database installed. You can do this by installing a mongodb docker container or by creating a remote database in [MongoDB Atlas](https://www.mongodb.com/cloud/atlas). 

## MongoDB configuration

After that, yous must reference this database in the `server.js` file.

```javascript
mongoose.connect(
    "mongodb://[DATABASE IP or URL]/nodeapi", 
    {useNewUrlParser: true, 
    useUnifiedTopology: true}
);
```
