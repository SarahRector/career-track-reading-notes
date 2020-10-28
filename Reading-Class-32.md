# Context API
https://reactjs.org/docs/context.html

* designed to share data that can be considered "global" for a tree of React components

* typically used when some data needs to be accessible by many components at different nesting levels

* React.createContext is the API
  * default value is only used when a component does not have a matching Provider above it in the tree
    * helpful for testing components in isolation without wrapping them

* if updating context is necessary, you can pass down a function that allows consumers to update the context

* could trigger unintentional renders in consumers when a providers parent re-renders
