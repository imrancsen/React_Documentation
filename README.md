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

        a) Functional Components      b) Class Components
        
        a)  Functional Components:
        These are javascript functions and can be created by writing a javascript function. For e.g.:
```
function Hello=()=>
{
    return <h1>Hello World!</h1>;
}
```
    

