# lambda-edge-response
A lightweight response payload builder for lambda@edge

## Installation

```
  npm install lambda-edge-response
```
or
```
  yarn add lambda-edge-response
```

## Usage

```js
  const response = require('lambda-edge-response');

  module.exports.handler = (event, context, callback) => callback(null, response({
    statusCode: 200,
    headers: {
      'Content-Type': 'application/json'
    },
    body: {
      hello: 'world'
    }
  }));
```
or

```js
  const response = require('lambda-edge-response');

  module.exports.handler = (event, context, callback) => callback(null, response({
    statusCode: 200,
    headers: {
      'Content-Type': 'text/plain'
    },
    body: 'Hello World'
  }));
```
