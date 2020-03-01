# webpack-basic-setup

### Install dependencies:
> npm install --save-dev webpack@next webpack-cli

### Create files:
#### 1. Create webpack.config.js at project root level.
```
// webpack.config.js
var path = require('path');

module.exports = {
  entry: path.resolve(__dirname, 'path/to/entry/file'),
  output: {
    path: path.resolve(__dirname, 'path/to/dist/folder'),
    filename: 'file_name'
  }
};
```

#### 2. Add new package script to run Webpack from config.
```
// package.json
{
  "scripts": {
      "build": "webpack" 
   }
}
```

### Run the webpack
> npm run build

NOTE:
Install latest node version.

// another way
"build": "webpack --mode development --config webpack.config.js"
