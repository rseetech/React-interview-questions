# React Interview Questions & Answers

   Here you will see Top 100 React Interview Questions & Answers for Fresher and experienced. 

   > Click :star:if you like the project and follow me on LinkedIn [@RameshKumar](https://www.linkedin.com/in/ramesh-kumar-choudhary/) for more updates. Coding React Project available at [React-Project](https://github.com/rseetech/routing-axios-search-counter-app-using-mui).


### Table of Contents

| No. | Questions                                                                                                                                                         |
| --- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1   | [Introduction to React](#introduction-to-react)                                         |
| 2   | [What is React?](#what-is-react?)                                                                                                             |
| 3   | [Features of React](#features-of-react)                                                        |
                              

1. ### Introduction to React

   React is an efficient, flexible, and open-source JavaScript framework library that allows developers to the creation of simple, fast, and scalable web applications. Jordan Walke, a software engineer who was working for Facebook created React. It was first deployed on the news feed of Facebook in 2011 and on Instagram in 2012. Developers from the Javascript background can easily develop web applications with the help of React.

   **[⬆ Back to Top](#table-of-contents)**

2. ### What is React?

   ReactJS is an open-source front-end JavaScript library for building user interfaces. ReactJS is maintained by Facebook and a community of individual developers and companies. It is widely used as a base in building single-page websites and mobile applications. It is very easy to use, and it allows users to create reusable UI components.

   **[⬆ Back to Top](#table-of-contents)**

3. ### Features of React

   1. **JSX :** JSX is an extension to javascript. Though it is not mandatory to use JSX in react, it is one of the good features and easy to use.

   2. **Components:** Components are like pure javascript functions that help make the code easy by splitting the logic into reusable independent code. We can use components as functions and components as classes. Components also have a state, props which makes life easy. Inside a class, the state of each of the props is maintained.
   
   3. **Virtual DOM:** React creates a virtual dom, i.e., in-memory data -structure cache. Only the final changes of DOM has later updated in the browsers DOM.

   4. **Javascript Expressions:** JS expressions can be used in the jsx files using curly brackets, for example {}.

   **[⬆ Back to Top](#table-of-contents)**

4. ### What are the major features of React?
   The major features of React are:
   1.	It uses VirtualDOM instead of RealDOM considering that RealDOM manipulations are expensive.
   2.	Supports server-side rendering. / server-side rendering (SSR)
   3.	Follows Unidirectional data flow or data binding.
   4.	Uses reusable/composable UI components to develop the view.

**[⬆ Back to Top](#table-of-contents)**

4. ### Advantages of ReactJS
   Here, are important pros/benefits of using ReactJS:

   1.	ReactJS uses virtual dom that makes use of in-memory data-structure cache, and only the final changes are updated in browsers dom. This makes the app faster.
   2.	You can create components of your choice by using the react component feature. The components can be reused and also helpful in code maintenance.
   3.	Reactjs is an open-source javascript library, so it is easy to start with.
   4.	ReactJS has become very popular in a short span and maintained by Facebook and Instagram. It is used by many famous companies like Apple, Netflix, etc.
   5.	Facebook maintains ReactJS, the library, so it is well maintained and kept updated.
   6.	ReactJS can be used to develop rich UI for both desktop and mobile apps.
   7.	Easy to debug and test as most of the coding is done in Javascript rather than on Html.
   8.	Easy to Learn and USe. ReactJS is much easier to learn and use. ...
   9.	Creating Dynamic Web Applications Becomes Easier. ...
   10. Reusable Components. ...
   11. Performance Enhancement. ...
   12. The Support of Handy Tools. ...
   13. Known to be SEO Friendly. ...
   14. The Benefit of Having JavaScript Library. ...
   15. Scope for Testing the Codes.


**[⬆ Back to Top](#table-of-contents)**

4. ### Disadvantages of ReactJS
   Here, are cons/ drawbacks of using ReactJS:
   1.	Most of the code is written in JSX, i.e., Html and css are part of javascript, it can be quite confusing as most other frameworks prefer keeping Html separate from the javascript code.
   2.	The file size of ReactJS is large.
   3.	The high pace of development. 
   4.	Poor Documentation.
   5.	View Part. 
   6.	JSX as a barrier.

**[⬆ Back to Top](#table-of-contents)**

4. ### What are Components in ReactJS?
Components are like pure javascript functions that help make the code easy by splitting the logic into reusable independent code.

**Functions Components**
Functional components are some of the more common components that will come across while working in React. These are simply JavaScript functions. We can create a functional component to React by writing a JavaScript function. These functions may or may not receive data as parameters. In the functional Components, the return value is the JSX code to render to the DOM tree.
```
test.jsx

import React from 'react';
import ReactDOM from 'react-dom';
function Hello() {
    return <h1>Hello, From RseeTech!</h1>;
} 
const Hello_comp = <Hello />;
export default Hello_comp;
```
```
index.js

import React from 'react';
import ReactDOM from 'react-dom';
import Hello_comp from './test.jsx';

ReactDOM.render(
    Hello_comp,
    document.getElementById('root')
);
```
**Class  Component**
React class based components are the bread and butter of most modern web apps built in ReactJS. These components are simple classes (made up of multiple functions that add functionality to the application). All class based components are child classes for the Component class of ReactJS. 
Here is a ReactJS example that uses a class as a component.
```
test.jsx

import React from 'react';
import ReactDOM from 'react-dom';

class Hello extends React. Component {
  render() {
    return <h1>Hello, From RseeTech!</h1>;
  }
}
export default Hello;
```
We can use Hello component in index.js file as follows:
```
index.js

import React from 'react';
import ReactDOM from 'react-dom';
import Hello from './test.jsx';

ReactDOM.render(
    <Hello />,
    document.getElementById('root')
);
```

**[⬆ Back to Top](#table-of-contents)**

4. ### ReactJS | Lifecycle of Components
Every React Component has a lifecycle of its own, lifecycle of a component can be defined as the series of methods that are invoked in different stages of the component’s existence.

•	**Initialization:** This is the stage where the component is constructed with the given Props and default state. This is done in the constructor of a Component Class.
•	**Mounting:** Mounting is the stage of rendering the JSX returned by the render method itself.
•	**Updating:** Updating is the stage when the state of a component is updated and the application is repainted.
•	**Unmounting:** As the name suggests Unmounting is the final step of the component lifecycle where the component is removed from the page.


1. **Initialization:** In this phase, the developer has to define the props and initial state of the component this is generally done in the constructor of the component. 
class Clock extends React.Component {
	constructor(props)
	{
		// Calling the constructor of
		// Parent Class React.Component
		super(props);
		
		// Setting the initial state
		this.state = { date : new Date() };
	}
}

 2. **Mounting:** Mounting is the phase of the component lifecycle when the initialization of the component is completed and the component is mounted on the DOM and rendered for the first time on the webpage.
•	componentWillMount() Function: As the name clearly suggests, this function is invoked right before the component is mounted on the DOM i.e. this function gets invoked once before the render() function is executed for the first time.
•	componentDidMount() Function: Similarly as the previous one this function is invoked right after the component is mounted on the DOM i.e. this function gets invoked once after the render() function is executed for the first time

3. **Updation:** React is a JS library that helps create Active web pages easily. Now active web pages are specific pages that behave according to their user.
componentWillRecieveProps() Function: This is a Props exclusive Function and is independent of States. This function is invoked before a mounted component gets its props reassigned. The function is passed the new set of Props which may or may not be identical to the original Props.
componentWillRecieveProps(newProps)

{
	if (this.props !== newProps) {
		console.log(" New Props have been assigned ");
		// Use this.setState() to rerender the page.
	}
}
•	**setState() Function:** This is not particularly a Lifecycle function and can be invoked explicitly at any instant. This function is used to update the state of a component. You may refer to this article for detailed information.
•	**shouldComponentUpdate() Function:** By default, every state or props update re-render the page but this may not always be the desired outcome, sometimes it is desired that updating the page will not be repainted. The shouldComponentUpdate() Function fulfills the requirement by letting React know whether the component’s output will be affected by the update or not.

•	**componentWillUpdate() Function:** As the name clearly suggests, this function is invoked before the component is rerendered i.e. this function gets invoked once before the render() function is executed after the updation of State or Props.
•	**componentDidUpdate() Function:** Similarly this function is invoked after the component is rerendered i.e. this function gets invoked once after the render() function is executed after the updation of State or Props.

4. **Unmounting:** This is the final phase of the lifecycle of the component that is the phase of unmounting the component              from the DOM. The following function is the sole member of this phase.
•	**componentWillUnmount() Function:** This function is invoked before the component is finally unmounted from the DOM i.e. this function gets invoked once before the component is removed from the page and this denotes the end of the lifecycle.
import React from 'react';
import ReactDOM from 'react-dom';

class Test extends React.Component {
	constructor(props)
	{
		super(props);
		this.state = { hello : "World!" };
	}

	componentWillMount()
	{
		console.log("componentWillMount()");
	}

	componentDidMount()
	{
		console.log("componentDidMount()");
}

	changeState()
	{
		this.setState({ hello : "Geek!" });
	}

	render()
	{
		return (
			<div>
			<h1>GeeksForGeeks.org, Hello{ this.state.hello }</h1>
			<h2>
			<a onClick={this.changeState.bind(this)}>Press Here!</a>
			</h2>
			</div>);
	}

	shouldComponentUpdate(nextProps, nextState)
	{
		console.log("shouldComponentUpdate()");
		return true;
	}

	componentWillUpdate()
	{
		console.log("componentWillUpdate()");
	}

	componentDidUpdate()
	{
		console.log("componentDidUpdate()");
	}
}

ReactDOM.render(
	<Test />,
	document.getElementById('root'));


**[⬆ Back to Top](#table-of-contents)**

4. ### Why we use JSX?
It is faster than regular JavaScript because it performs optimization while translating the code to JavaScript.
Instead of separating technologies by putting markup and logic in separate files, React uses components that contain both.
t is type-safe, and most of the errors can be found at compilation time.
It makes easier to create templates.

   **[⬆ Back to Top](#table-of-contents)**

4. ### Why can't browsers read JSX?
Browsers cannot read JSX directly because they can only understand JavaScript objects, and JSX is not a regular JavaScript object. Thus, we need to transform the JSX file into a JavaScript object using transpilers like Babel and then pass it to the browser.

   **[⬆ Back to Top](#table-of-contents)**

4. ### What do you understand by Virtual DOM?
A virtual DOM is a lightweight JavaScript object which originally is just a copy of the real DOM. It is a node tree that lists the elements, their attributes and content as Objects and their properties. React’s render function creates a node tree out of the React components. It then updates this tree in response to the mutations in the data model which is caused by various actions done by the user or by the system.


   **[⬆ Back to Top](#table-of-contents)**

4. ### How different is React’s ES6 syntax when compared to ES5?
Syntax has changed from ES5 to ES6 in the following aspects:

require vs import
// ES5
var React = require('react');
// ES6
import React from 'react';

export vs exports
// ES5
module.exports = Component;
// ES6
export default Component;


   **[⬆ Back to Top](#table-of-contents)**

4. ### What is the purpose of render() in React.
Each React component must have a render() mandatorily. It returns a single React element which is the representation of the native DOM component. If more than one HTML element needs to be rendered, then they must be grouped together inside one enclosing tag such as <form>, <group>,<div> etc. This function must be kept pure i.e., it must return the same result each time it is invoked.

   **[⬆ Back to Top](#table-of-contents)**

4. ### How can you embed two or more components into one?
We can embed components into one in the following way:

class MyComponent extends React.Component{
    render(){
        return(          
             
<div>
               
<h1>Hello</h1>
 
                <Header/>
            </div>
 
        );
    }
}
class Header extends React.Component{
    render(){
        return
 
<h1>Header Component</h1>
   
   };
}
ReactDOM.render(
    <MyComponent/>, document.getElementById('content')
);

   **[⬆ Back to Top](#table-of-contents)**

4. ### What is Props?

rops is the shorthand for Properties in React. They are read-only components which must be kept pure i.e. immutable. They are always passed down from the parent to the child components throughout the application. A child component can never send a prop back to the parent component. This help in maintaining the unidirectional data flow and are generally used to render the dynamically generated data.

   **[⬆ Back to Top](#table-of-contents)**

4. ### What is state in React?

State of a component is an object that holds some information that may change over the lifetime of the component. We should always try to make our state as simple as possible and minimize the number of stateful components.

class User extends React.Component {
  constructor(props) {
    super(props)

    this.state = {
      message: 'Welcome to React world'
    }
  }

  render() {
    return (
      <div>
        <h1>{this.state.message}</h1>
      </div>
    )
  }
}

![Alt text](image-1.png)

   **[⬆ Back to Top](#table-of-contents)**

4. ### What is the difference between state and props?

Both props and state are plain JavaScript objects. While both of them hold information that influences the output of render, they are different in their functionality with respect to component. Props get passed to the component similar to function parameters whereas state is managed within the component similar to variables declared within a function.

   **[⬆ Back to Top](#table-of-contents)**

4. ### Why should we not update the state directly?
If you try to update state directly then it won't re-render the component.
**//Wrong**
this.state.message = 'Hello world'
Instead use setState() method. It schedules an update to a component's state object. When state changes, the component responds by re-rendering.
**//Correct**
this.setState({ message: 'Hello World' })

   **[⬆ Back to Top](#table-of-contents)**

4. ### What are synthetic events in React?
SyntheticEvent is a cross-browser wrapper around the browser's native event. It's API is same as the browser's native event, including stopPropagation() and preventDefault(), except the events work identically across all browsers.

   **[⬆ Back to Top](#table-of-contents)**

4. ### What is the use of refs?
The ref is used to return a reference to the element. They should be avoided in most cases, however, they can be useful when you need a direct access to the DOM element or an instance of a component.
class MyComponent extends React.Component {
  constructor(props) {
    super(props)
    this.myRef = React.createRef()
  }
  render() {
    return <div ref={this.myRef} />
  }
}


   **[⬆ Back to Top](#table-of-contents)**

4. ### What are Higher-Order Components?

A higher-order component (HOC) is a function that takes a component and returns a new component. Basically, it's a pattern that is derived from React's compositional nature.

We call them pure components because they can accept any dynamically provided child component but they won't modify or copy any behavior from their input components.
const EnhancedComponent = higherOrderComponent(WrappedComponent)

HOC can be used for many use cases:
i.	   Code reuse, logic and bootstrap abstraction.
ii.	Render hijacking.
iii.	State abstraction and manipulation.
iv.	Props manipulation.

   **[⬆ Back to Top](#table-of-contents)**

4. ### What is context?
Context provides a way to pass data through the component tree without having to pass props down manually at every level.
For example, authenticated user, locale preference, UI theme need to be accessed in the application by many components.
const {Provider, Consumer} = React.createContext(defaultValue)

   **[⬆ Back to Top](#table-of-contents)**

4. ### How to write comments in React?
The comments in React/JSX are similar to JavaScript Multiline comments but are wrapped in curly braces.
**Single-line comments:**
<div>
  {/* Single-line comments(In vanilla JavaScript, the single-line comments are represented by double slash(//)) */}
  {`Welcome ${user}, let's play React`}
</div>
**Multi-line comments:**
<div>
  {/* Multi-line comments for more than
   one line */}
  {`Welcome ${user}, let's play React`}
</div>


   **[⬆ Back to Top](#table-of-contents)**

4. ### What are fragments?

It's common pattern in React which is used for a component to return multiple elements. Fragments let you group a list of children without adding extra nodes to the DOM.
render() {
  return (
    <React.Fragment>
      <ChildA />
      <ChildB />
      <ChildC />
    </React.Fragment>
  )
}
There is also a shorter syntax, but it's not supported in many tools:
render() {
  return (
    <>
      <ChildA />
      <ChildB />
      <ChildC />
    </>
  )
}

**[⬆ Back to Top](#table-of-contents)**

4. ### Why fragments are better than container divs?
Below are the list of reasons,
i.	Fragments are a bit faster and use less memory by not creating an extra DOM node. This only has a real benefit on very large and deep trees.
ii.	Some CSS mechanisms like Flexbox and CSS Grid have a special parent-child relationships, and adding divs in the middle makes it hard to keep the desired layout.
iii.	The DOM Inspector is less cluttered.

   **[⬆ Back to Top](#table-of-contents)**
