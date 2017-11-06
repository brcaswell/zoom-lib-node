# Zoom Library for Node.js

> This library is for Version 1 of the [Zoom API](https://zoom.github.io/api-v1/)

## Getting started

### Install

You can install this package with `npm`

`npm install zoomus`

### Documentation

Documentation is available on the [Zoom REST API docs site](https://zoom.github.io/api-v1/?javascript)


### Quick Start

```javascript
//include the zoom library
var Zoom = require("zoomus")({
    "key" : "<api_key>",
    "secret" : "<api_secret>"
});

//create a user
var user = {
    email: 'user@domain.com',
    type: 1
};

Zoom.user.create(user, function(res){
    if(res.error){
        //handle error
    } else {
        //res is user object
        console.log(res);     
    }
});
```