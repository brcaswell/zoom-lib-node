# Zoom Library for Node.js

## Getting started

### Install

You can install this package with `npm`

`npm install zoomus`

### Documentation

Documentation is available on the [Zoom REST API docs site](https://zoom.github.io/api)


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

Zoom.user.create(user, function(err, res){
    if(err){
        //handle error
    } else {
        //res is user object
        console.log(res);     
    }
});
```