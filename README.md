transitsms.js
=============

Node wrapper for Transit SMS API. Uses `request` to make API calls and `Q` to manage callbacks

TODO: Write test scripts & validate inputs & set defaults

### Usage
```
var transitsms = require('transitsms')({
  apiKey: XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX,
  secret: XXXXXXXXXXXXXXXXXXXXXXXXXXXXX
});

transitsms.send({
  to: 00000000000,
  message: 'Yo'
}).then(function(data) {
  console.log('Hey I'm Working!');
}).catch(function(err) {
  console.log('Boo, something bad happened')
});
````
