# React-Styling
```js
import React from "react";
import ReactDOM from "react-dom";

let greeting;

const date = new Date();
const currentTime = date.getHours();

const customStyle = {
  color: ""
};

if (currentTime < 12) {
  greeting = "Good Morning";
  customStyle.color = "darkgreen";
} else if (currentTime < 18) {
  greeting = "Good Afternoon";
  customStyle.color = "teal";
} else {
  greeting = "Good Evening";
  customStyle.color = "slategray";
}

ReactDOM.render(
  <h1 className="heading" style={customStyle}>
    {greeting}
  </h1>,
  document.getElementById("root")
);
```
Created with CodeSandbox
