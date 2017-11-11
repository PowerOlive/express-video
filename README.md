# DaVideo 1.0.1
A video streaming middleware for express.js

**Note:** Currently, this can only stream files in .mp4 format.

## Usage
Installation: `npm install davideo --save`

Code Sample:
```javascript
const express = require('express');
const path = require('path');
const davideo = require('davideo');
const app = express();

app.use('/videos', davideo.stream(path.join(__dirname, 'videos'))); // Pass the folder with the videos you'd like to stream

app.listen(3000, function () {
  console.log('Listening on port 3000!');
});

```
