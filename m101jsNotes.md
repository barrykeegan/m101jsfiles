

# M101JS Notes

##Week 1:

###What is MongoDB

###Overview of Building App with MongoDB

###Installing
On Arch: 

    # pacman -S mongodb mongodb-tools

###JSON
Javascript Object Notation.

Key/Value pairs.

Types: String, Number, Boolean, Array, Objects.

[json.org](http://www.json.org) for further


###BSON
Binary JSON

Binary data superset of JSON.

MongoDB uses BSON

Lightweight/Traversable/Efficient

Types: String, Byte, Integer, Double, Date, Boolean, Array, Object, Binary Data

[bsonspec.org](http://www.bsonspec.org/)

###Intro to Creating and Reading Documents
CRUD - Create, Read, Update, Delete

From Mongo Shell:
To Manually Run mongod: $ mongod --dbpath */path/to/db*

To see dbs: show dbs

To switch to video database: use video

To add a document to movies collection (returns document): db.**movies**.insertOne({***"key"***: ***"value"***, ...})

To find all documents in the movies collection (returns cursor): db.**movies**.find()[.pretty()]

To find a single document in the movies collection:
db.**movies**.findOne()[.pretty()]


###Installing Node.js
On Arch: # pacman -S nodejs npm

###Hello World Node.js
Method 1:

1. console.log("Hello, World"); >> app.js
2. node app.js

Method 2:

1. var http = require('http');
2. var server = http.createServer(function (request, response) {
3. response.writeHead(200, {"Content-Type": "text/plain"});
4. response.end("Hello, World\n");
5. });
6. server.listen(8888);
7. console.log("Server running at http://localhost:8888");
8. node app.js

###Intro to npm
For local installs: npm install *packageName*. Installs into node_modules directory.

For global installs: npm install -g *packageName*. Installs for whole system.

###Intro to Node.js Driver


###Hello World using Express
###Hello World using Templates
###All Together Now
###Express: Handling GET Requests
###Express: Handling POST Requests
###Intro to Course project
##Week 2:
