# React_Documentation
## 1.React Basics

- #### What is React.js?
React was originally created by Jordan Walke, a software engineer at Facebook in 2012 and later open-sourced in 2013. It is a Javascript Library for building user interfaces which uses componets (small pieces of codes) to make complex UI. 
Developers when using React are able to create large web applications which use data needed to change over time, without refreshing the page resulting in faster and better web apps. The popular platforms using react are: Facebook, Dropbox, whatsapp, netflix etc.



- #### How to set up required tools to develop web applications with React?
We need to install few softwares before creating web applications with React. These softwares/tools can easily be googled.

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
Now we are ready to write lines for our first react app.



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
