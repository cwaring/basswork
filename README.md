# Basswork

Rework wrapper for use with [Basscss](http://basscss.com)

## Rework Plugins Used:
- Rework NPM
- Rework Custom Media
- Rework Vars
- Rework Calc
- Rework Plugin Colors

## Install

```
npm install basswork
```

## Usage
Pass an unprocessed CSS string to Basswork, which will return the processed CSS.

```javascript
var basswork = require('basswork');
var fs = require('fs');

var src = fs.readFileSync('./src/base.css', 'utf8');
var css = basswork(src);
fs.writeFileSync('./css/base.css', css);
```

Or from the command line:

```sh
$ basswork --sourcemap in.css > out.css
```
