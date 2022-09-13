# React_Documentation
## 1.React Basics

- #### What is React.js?
React was originally created by Jordan Walke, a software engineer at Facebook in 2012 and later open-sourced in 2013. It is a Javascript Library for building user interfaces and uses componets (small pieces of codes) to make complex UI. 
Developers when using React are able to create large web applications which use data needed to change over time, without refreshing the page resulting in faster and better web apps. The popular platforms using react are: Facebook, Dropbox, whatsapp, netflix etc.



- #### How to set up required tools to develop web applications with React?
To use react properly we need to install following softwares/apps before creating web applications with React. These softwares/tools can easily be googled:

i.
Install VS Code (a source code editor by Microsoft).

ii.
Install Nord.js which is a back-end JavaScript runtime environment and execute codes outside a web browser. NPM is complementary with Nord.js, it accomapnies nord.js.

iii.
Add extension to Chrome: React Development Tools
It will show the state of your components.

iv.
A few extensions for VS Code for the convenience and ease of use:

    a) Thuderclient             b) ES7 React/Redux/GraphQL/React-Native snippets
    
    c) Bracket Pair Colorizer   d) Auto Rename Tag
    
    d) Live server
Now we are ready to write code for our first react app.



- #### What is React JSX??
JSX stands for JavaScript XML which allows developer to write HTML in React. It converts HTML tags into react elements.
Example:
```
const myelement1 = <h1>Hello Earth</h1>;
```


- #### What are components in react?
Compononents are building blocks of React. In simple words, any application developed using React is composed of small pieces called components. Through this the process of making UIs become easier. We can work on these individual process separately and then merge them to get final version of our UI. Below is an example image of airbnb site shown in components:
![courtesy:betterprogramming.pub](https://miro.medium.com/max/875/1*qpygBsXUnYiuFrZTcX65gA.png)

There are mainly two types of React components:
        a) Functional Components  b) Class Components
        
        a)  Functional Components
        These are javascript functions and can be created by writing a javascript function. For e.g.
```
myfunction Hello=()=>
{
    return <h1>Hello World!</h1>;
}
```
    
        
        b)  Class Components
        The class components, unlike function components, can work with each other.
        The data from one class component can be passed to other class components.
        It uses 'extends React.Component' when initiating class component. For e.g.
```
class myfunction extends React.Component 
{
    return <h1>Hello World!</h1>;
}
```


- #### How to create a new react app?
    First we shall open VS code and create a folder where all the necessary files for app will be stored.
    or
    Alternatively, we can first create our React working directory through windows explorer, and right click within the folder and select option to open with VS code. Then follow the following steps:
    1. Write the following command in VS code terminal:
    ```bash
    npx create-react-app imr-app
    ```
    It maytake some time so we need to wait patiently. After succesful creation, it will make a folder namely 'imr-app' and all the necessarry files/folders inside it. Our main folder where we edit will be 'SRC'.    
    
    2. To run the app, you need to stay within the app folder or use proper path with the following command:
    ```bash
    npm start
    ```
    If you are running it for the first time, it will ask you some firewall permissions for nord etc and will run at "http://localhost:3000/" in the browser.
    
    
    
    
## 2.React State & Events 

- #### What is React State?
State is a javascript object used by React to store data/property of the component and may change overtime. It is a built-in object.
- #### Demonstration of state in react app
As we know that the state is a built-in React object and contains data or information about the component. The following example can explain how we can use these:
```bash
class Colour extends React.Component {
  constructor() {
    super();
    this.state = {
      Type: "Crayons",
      colour: "blue",
    };
  }
  render() {
    return (
      <div>
        <h1>The type of color is {this.state.type}</h1>
        <h2>The color is {this.state.colour}</h2>
      </div>
    );
  }
}
```
- #### What is an event?
Event is an action that can be triggered by user or system. Events in react are same as in HTML. Some of the examples are:
![reactevent](https://user-images.githubusercontent.com/97589134/185609113-f8ac8151-18d3-463b-a5a7-5b26c3a18eae.png)
Beside this there are plent of more events in react which can be used as and when required.

- #### How are events handled in react?
Event handling allows users to communicate with a webpage and perform the desired task when some speific event like a click or right click etc happens. Events are triggered when user do certain actions like pressing key, hovering mouse, clicking etc. So the web-page/application must be able to handle such actions i.e events and execute the code. Whilre creating events, we also need to keep these rules in mind:

i.camelCase Convention: Instead of using lowercase we use camelCase while giving names of the react events. That simply means we write ‘onClick’ instead of ‘onclick’.

ii.Pass the event as a function: In React we pass a function enclosed by curly brackets as the event listener or event handler, unlike HTML where we pass the event handler or event listener as a string.

iii.Prevent the default: Just returning false inside the JSX element does not prevent the default behavior in react. Instead, we have to call the ‘preventDefault’ method directly inside the event handler function.(source for the rules: geeksforgeeks)

for example button on click in react will be written as follows:
```bash
<button onClick={testMe}>
 Test me
</button>
```

- #### Demonstration of react event 

import React from 'react';
import ReactDOM from 'react-dom/client';

function carStart() {
  const start = () => {
    alert("Engine Started!");
  }

  return (
    <button onClick={start}>start engine!</button>
  );
}

const root = ReactDOM.createRoot(document.getElementById('root'));
root.render(<carStart />);
