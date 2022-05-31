# JSON Server

- Get a full fake REST API with zero coding in less than 30 seconds (seriously).

- Created with <3 for front-end developers who need a quick back-end for prototyping and mocking.



## Install JSON Server

npm install -g json-server



## Create a db.json file with some data

{
  "posts": [
    { "id": 1, "title": "json-server", "author": "typicode" }
  ],
  "comments": [
    { "id": 1, "body": "some comment", "postId": 1 }
  ],
  "profile": { "name": "typicode" }
}



## OR

## Start JSON Server

json-server --watch db.json



### Full information github learn

https://github.com/typicode/json-server/blob/master/README.md

### Youtube Video

https://youtu.be/u7dPGuGB0Kc
