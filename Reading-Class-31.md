# Building Your Own Hooks
https://reactjs.org/docs/hooks-custom.html

* custom hooks are functions whose name starts with "use" and may call other Hooks
  * we can decide what it takes as arguments and what it should return
* every time you use a custom hook, all state and effects inside of it are fully isolated

# Rules of Hooks
https://reactjs.org/docs/hooks-rules.html

* only call hooks at the top level
  * not inside loops or anything nested
* only call hooks from react functions
  * can only call them from react function components and custom hooks

# The Guide to Learning React Hooks (Examples & Tutorials)
https://www.telerik.com/kendo-react-ui/react-hooks-guide/#toc-custom-react-hooks

* useContext can be used to pass props around

* this is a really good article that gives very thourough examples on the different hooks you can use and ways to use them

# 10 React Hooks you Should Have in Your Toolbox
https://blog.bitsrc.io/10-react-custom-hooks-you-should-have-in-your-toolbox-aa27d3f5564d

* useArray: provides array manipulation methods
* react-use-form-state: allows you to simplify forms
* react-fetch-hook: makes a fetch
* useMedia: tracks state of CSS media query
* react-useportal hook: render children into a DOM node that exists outside the DOM heirarchy
* react-firebase-hooks: something to do with auth
* use-onClickOutside hook: not really sure what this does....
* useIntersectionObserver: also not sure about this one
* use-location hook: gets location of browser
* use-redux hook: returns store and dispatch property

