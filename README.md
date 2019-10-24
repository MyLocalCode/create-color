# Create color

[![npm version](https://badge.fury.io/js/create-color.svg)](https://badge.fury.io/js/create-color) ![](https://img.shields.io/npm/dm/create-color.svg)

A tiny (590 B) JavaScript library to generate the permanent color from any string, array or object.

## Install

```bash
npm install create-color
// or
yarn add create-color
```

## Usage

```js
const createColor = require("create-color");
// or
import createColor from "create-color";
```

```js
// format by default: hex
const hex = createColor("canThereBeAnyText"); // => "#67cb22"
```

```js
// from string
const hsl = createColor("canThereBeAnyText", { format: "hsl" }); // => "hsl(96,71%,46%)"

// from object
const hex = createColor(
  { name: "Andrey", age: 27, role: "user" },
  { format: "hex" }
); // => "#f6555d"

// from array
const rgb = createColor(["random", "color", "generation"], { format: "rgb" }); // => "rgb(218,179,136)"
```

