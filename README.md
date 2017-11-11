# DaVideo 1.0.0
A video streaming middleware for express.js

**Note:** Currently, this can only stream files in .mp4 format.

## Usage
Installation: `npm install davideo --save`

Code Sample:
```javascript
const express = require('express');
const app = express();
const davideo = require('davideo');

app.use('/videos', davideo); // Pass the path of the folder with the .mp4 files you'd like to stream

app.listen(3000, function () {
  console.log('Listening on port 3000!');
});

```
