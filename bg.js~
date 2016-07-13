var express = require('express');
var bodyParser = require('body-parser');
var app =  express();

app.get('/test', function(req, res){
  res.send('Hello World!');
  app.use(bodyParser.json());  
});

app.post('/users', function(req, res){
  app.use(bodyParser.json());
  app.use(bodyParser.urlencoded({     // to support URL-encoded bodies
  extended: true
}));
  console.log(req.body['username']);
});

app.listen(3000);

