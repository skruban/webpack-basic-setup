# webpack-basic-setup

Install (locally):
>yarn add webpack@next webpack-cli --dev

To run Webpack:
1.
Create webpack.config.js at project root level.
// webpack.config.js
var path = require('path');

module.exports = {
  entry: path.resolve(__dirname, 'path/to/entry/file'),
  output: {
    path: path.resolve(__dirname, 'path/to/dist/folder'),
    filename: 'file_name'
  }
};


2.
Add new package script to run Webpack from config.
// package.json
{
  "scripts": {
      "start": "webpack --mode development --config webpack.config.json" 
   }
}


Run:
> yarn start


NOTE:
Install latest node version.
