# md5-promised
Handle file hashing from the promise framework.
- Provide a hashEncoding or use the default 'hex'.

## Getting Started

```shell
npm install exec-promised --save
```

## Example hashing a the md5-promised index.js (v1.0.0)
```js
var hash = require('md5-promised');
hash('md5-promised/index.js').then(function(md5) {
  console.log('md5-promised hash is:', md5);//67206318cc1a0914166213140c19b4d8
}).fail(function(err) {
  console.log('Could not hash', err, err.stack);
});
```