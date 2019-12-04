# React-IcoMoon

[![License](https://img.shields.io/badge/License-Apache%202.0-green.svg)](http://www.apache.org/licenses/LICENSE-2.0.html)


![React-Icomoon Logo](logo.png)

**Size < 2kb** and **0 Dependency**

With React-Icomoon you can easily use the icons you have selected or created in icomoon.

<!-- ## [Demo](https://codesandbox.io/s/github/aykutkardas/react-icomoon-playground) -->

## Install

```
npm install react-icomoon
```

## Usage

You can use the icons you selected on IcoMoon by downloading the **selection.json** file.

https://icomoon.io/app/

### Declare
```js
// icon.js
import React from "react";
import IcoMoon from "react-icomoon";
const iconSet = require("./selection.json");

const Icon = ({ ...props }) => {
  return <IcoMoon iconSet={iconSet} {...props} />;
};

export default Icon;
```
### Use
```js
import Icon from "./icon";

<Icon icon="focus" />
```

## Props List
| Name              | Type          | Default   | Sample                        |
|-------------------|---------------|-----------|-------------------------------|
| iconSet           | Object        | undefined | "selection.json file content" |
| icon              | String        | undefined | "home"                        |
| size              | Number,String | undefined | "1em", 10, "100px"            |
| style             | Object        | {...}     | { color: '#ff0'}              |
| className         | String        | undefined | "icomoon"                     |
| disableFill       | Boolean       | undefined | true                          |
| removeInlineStyle | Boolean       | undefined | true                          |


### Default Style
```js
{
  display: "inline-block",
  stroke: "currentColor",
  fill: "currentColor",
}
```