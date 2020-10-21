# Architectural Styles and Architectural Patterns
https://medium.com/@mlbors/architectural-styles-and-architectural-patterns-c240f7df88a0#:~:text=Architectural%20Patterns%20VS%20Design%20Patterns&text=In%20a%20few%20words%2C%20while,and%20mechanisms%20of%20a%20system.

* architectural pattern is a reusable solution to a recurring problem

* Architectural patterns and pattern styles can be layered 
  * presentation/UI
  * application or service
  * buisness logic or domain
  * data access or persistence

* MVC is layered architecture

# Container and Presentation Pattern
https://alchemycodelab.github.io/fsjs-notes/05_react/patterns/container_presentation/

* container components are connected with how things work (manage state, fetch from APIs, event handlers, etc)

* presentation components are concerned with how things look (receive props and use those props to render and style DOM)

# Container Component Details
https://alchemycodelab.github.io/fsjs-notes/05_react/patterns/container_presentation/container-details

* are Class based

* use this.setState to set the state inside a class based container

* can also be used as custom hooks rather than as components

# Presentation Component Details
https://alchemycodelab.github.io/fsjs-notes/05_react/patterns/container_presentation/presentation-details

* written as functional components

* need to pass props in, use PropTypes

# Functional vs Class-Components in React
https://medium.com/@Zwenza/functional-vs-class-components-in-react-231e3fbd7108

* can define a react component by writing a JavaScript function or by using ES6 Class syntax

* can't use setState() in a functional component - stateless

* functional components are easier to read
* less code
* easier to seperate container and presentational components
* performance boost for functional components in future react versions

# Conditional Rendering
https://reactjs.org/docs/conditional-rendering.html

* can use conditionals to render to the DOM in react 

* can embed expressions in JSX by wrapping them in curly braces
