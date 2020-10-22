# Model-View-Controller
https://en.wikipedia.org/wiki/Model%E2%80%93view%E2%80%93controller

* used to seperate internal logic from the way things are presented to the user

* Model: apps dynamic data structure (data, logic, rules)

* View: the way the info is presented

* Controller: converter for model and view. Takes input and converts it.

# The 4 Layers of Single Page Applications You Need to Know
https://hackernoon.com/architecting-single-page-applications-b842ea633c2e

* React, Angular and Vue are declarative
* State is every piece of data that changes in an app

# A Model View Controller Pattern for React
https://blog.testdouble.com/posts/2019-11-04-react-mvc/

* MVC thought of as "server-side-architecture"

* but we should think more broadly
    * could be great for React

# Reconciliation
https://reactjs.org/docs/reconciliation.html

* render() creates a tree of React elements
* each time the app re-renders, that tree is eliminated and a new tree is made
* React uses keys to match children in the origional tree with children in the subsequent tree
