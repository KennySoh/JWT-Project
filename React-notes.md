## What is React 
A Javascript library for building user interface. Browser-based.  
  
### Works in Components   
![Image](https://github.com/KennySoh/JWT-Project/blob/master/pic/react1.png) 

### First React Code
Normally u keep repeating code with html, React allow use to create reusable component.    

![Image](https://github.com/KennySoh/JWT-Project/blob/master/pic/react2.png)  


JS (Babel)
```
// JS Babel used -> Allow u to use JSX syntax -> Allow compliation of react codes.
function Person(){
  return (
    <div class="person">
      <h1>{props.name}</h1>
      <p>Your Age: {props.age}</p>
    </div>
  );
}

/*-------First way of rendering multiple React Componenets------------*/
ReactDOM.render(<Person name="Max" age="28"/>, document.querySelctor("#p1");
ReactDOM.render(<Person name="Manu" age="31"/>, document.querySelctor("#p2");

/*-------Second way of rendering multiple React Componenets------------*/
var app=(
  <div> //Have to wrap with div, 
    <Person name="Max" age="28"/>
    <Person name="Manu" age="31"/>
  </div>
);

ReactDOM.render(app, document.querySelctor("#app");

```
  
Html  
```
<div id="p1"></div>
<div id="p2"></div>

<div id="app"></div>
```
### Why Should we Choose React
***
- UI state becomes difficult to handle with Vanilla Javacript
- Focus on Business Logic, not on preventing your App from exploding
- Huge Ecosystem.... 
***

### Single Page Applications vs Multi Page Applications
![Image](https://github.com/KennySoh/JWT-Project/blob/master/pic/react3.png) 

## Course Overview
***
- The Basics
- Debugging
- Styling Components
- Componeents Deep Dive
- HTTP Requests
- Routing 
- Forms & Validation
- Redux
- Authentication
- Testing Introduction
- Deployment
- Bonus ( Animation, Webpack)
***

### 
