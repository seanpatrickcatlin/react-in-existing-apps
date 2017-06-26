# Using React in Existing Web Applications
## Sean Catlin

---

# Introduction
## Sean Catlin
### catlin.sean@gmail.com
### seancatlin.com

---

# Overview
1. Introduction to React
1. New React application
1. Using React in an existing application

---

# Motivation
* React is just javascript
* React is not a framework
* React can be used in existing applications

---

# What is React?
A JavaScript library for building user interfaces.

---

# Why use React?
* It's the new(<i>ish</i>) hotness
* Performance (virtual dom)
* Support (made by facebook)
* Community (very popular)
* Declaritive/functional/immutable
* Introduction to other libraries and frameworks such as React Native

---

# State vs props
## State
Managed by each react component, local to that component.
## Props
Received by each react component.

---

# React component lifecycle
### componentWillMount
### componentDidMount
### componentWillReceiveProps
### componentWillUpdate
### shouldComponentUpdate
### render (**REQUIRED**)
### componentDidUpdate
### componentWillUnmount

---

# How to use react in a new application
**tldr**: use create-react-app
1. Install node
1. Install create-react-app
```
npm install -g create-react-app
```
3. Create a new application with create-react-app
```
create-react-app my-app
```
4. Run your react app
```
cd my-app/
npm start
```
5. ???
1. Profit
1. **Bonus** Install the [React Developer Tools](https://github.com/facebook/react-devtools)

---

# But I have an existing application
## No Worries!!!
React simply manages the children of a single DOM element.  All you need is an empty element in your html and you can use react to render your code.
```
<div class="myreactapp"></div>
```

---

# ReactDom.render()
// TODO

---

# CDN

---

# JSX

Extremely helpful, highly recommended, but not necessary.

The React docs even state [link](https://facebook.github.io/react/docs/react-without-jsx.html)

> JSX is not a requirement for using React. Using React without JSX is especially convenient when you don't want to set up compilation in your build environment.
>
> Each JSX element is just syntactic sugar for calling React.createElement(component, props, ...children). So, anything you can do with JSX can also be done with just plain JavaScript.

Try it for yourself on the [babel repo](https://babeljs.io/repl/#?babili=false&evaluate=true&lineWrap=false&presets=es2015%2Creact%2Cstage-0&code=function%20hello()%20%7B%0A%20%20return%20%3Cdiv%3EHello%20world!%3C%2Fdiv%3E%3B%0A%7D)

---

# But what about State Management?
1. Flux
1. Redux
1. MobX

Redux is an amazing tool, I use it every day at work.  When learning React I would highly recommend to completely wrap your head around React, including state, props, and the component lifecycle before integrating Redux into your application

 Redux was officially introduced in July 2015 by Dan Abramov (aka gaeron) in the React.Europe talk ["Hot Reloading with Time Travel"](https://www.youtube.com/watch?v=xsSnOQynTHs) and quickly became the recommended state management system for React.  In 2016 he wrote the very insightful article ["You might not need redux."](https://medium.com/@dan_abramov/you-might-not-need-redux-be46360cf367) in which he states

> Redux offers a tradeoff. It asks you to:
> * Describe application state as plain objects and arrays.
> * Describe changes in the system as plain objects.
> * Describe the logic for handling changes as pure functions.
>
> None of these limitations are required to build an app, with or without React. In fact these are pretty strong constraints, and you should think carefully before adopting them even in parts of your app.

---

# Demo

todomvc-jquery

chucknorris.io

---

# Conclusion
React gives you great possibilities and can even be used in existing applications and is not limited to only being used in new applications.

---

# Questions
AM(**A**)A [ask me <i>almost</i> anything]

# Fin
## The End
* View this slide deck [gitpitch.com/seanpatrickcatlin/react-in-existing-applications](
https://gitpitch.com/seanpatrickcatlin/react-in-existing-apps) 
* View the source [github.com/seanpatrickcatlin/react-in-existing-applications](https://github.com/seanpatrickcatlin/react-in-existing-apps)
* FDR