# Understanding React 'setState'
https://css-tricks.com/understanding-react-setstate/

* react components with state render UI based on that state, when state changes so does UI

* setState is the only way to deal with state after the initial state set up

* reconciliation is the way that React updates the DOM

# React Lists and Keys
https://reactjs.org/docs/lists-and-keys.html

* can build collections of elements and include them in JSX using curly braces

* can set an array and loop through it using .map, then return a <li> element for each items and assign that array to listItems. Then, include entire listItems array inside a <ul> element and render it to the DOM

* can also render elements inside of a component
  * needs a **key** (special string attribute)
    * needs to be unique, most often you would use ids from your data

# Typechecking with PropTypes
https://reactjs.org/docs/typechecking-with-proptypes.html

* can use things like TypeScript to check props but React also has PropTypes built in

* can check type, default props, and specify that only a single child can be passed to a component as children

# Components and Props
https://reactjs.org/docs/components-and-props.html

* components split up the app into smaller pieces

* functions and classes are both components

* components can be rendered as either DOM tags or user-defined components

# Handling Events
https://reactjs.org/docs/handling-events.html

* React events are camelCase

* pass a function as the event handler, rather than a string

* cant return false, have to call preventDefault explicitly

# Snapshot Testing
https://jestjs.io/docs/en/snapshot-testing

* basically takes a picture and compares it to another

* can be used to test React UI to make sure it hasn't unexpectedly changed

* snapshot tests can fail when you change something on purpose. To update the test run 
```jest --updateSnapshot```

* can also use watch mode to run interactive snapshot

# React Testing Library
https://kentcdodds.com/blog/introducing-the-react-testing-library

* a replacement for enzyme

* tests resemble how a user uses your application

* doesn't have utilities that enable testing implementation details, focuses on providing utilities that encourage good testing and software practices.
