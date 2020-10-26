# Hooks at a Glance
https://reactjs.org/docs/hooks-overview.html

* let you use state without writing a class

* useState sets the initial state
  * you can use it more than once in a single component
  ```js
  function ExampleWithManyStates() {
  // Declare multiple state variables!
  const [age, setAge] = useState(42);
  const [fruit, setFruit] = useState('banana');
  const [todos, setTodos] = useState([{ text: 'Learn Hooks' }]);
  // ...
}```

* useEffect serves same purpose as componentDidMount, componentDidUpdate, etc 

* When you call useEffect, you’re telling React to run your “effect” function after flushing changes to the DOM. Effects are declared inside the component so they have access to its props and state.

* two rules of hooks:
  * only call hooks at the top level (not inside loops, conditions or nested functions)
  * only call hooks from React function components not from regular JS functions

  # Using the State Hook
  https://reactjs.org/docs/hooks-state.html

  * have to import useState from react

  * What does calling useState do? It declares a “state variable”. Our variable is called count but we could call it anything else, like banana. This is a way to “preserve” some values between the function calls — useState is a new way to use the exact same capabilities that this.state provides in a class. Normally, variables “disappear” when the function exits but state variables are preserved by React.

# Using the Effect Hook
https://reactjs.org/docs/hooks-effect.html

* allows you to replace componentDidMount, etc

* What does useEffect do? By using this Hook, you tell React that your component needs to do something after render. React will remember the function you passed (we’ll refer to it as our “effect”), and call it later after performing the DOM updates. In this effect, we set the document title, but we could also perform data fetching or call some other imperative API.

* 
```js
import React, { useState, useEffect } from 'react';

function Example() {
  const [count, setCount] = useState(0);

  useEffect(() => {
    document.title = `You clicked ${count} times`;
  });

  return (
    <div>
      <p>You clicked {count} times</p>
      <button onClick={() => setCount(count + 1)}>
        Click me
      </button>
    </div>
  );
}
```

# Hooks API Reference
https://reactjs.org/docs/hooks-reference.html

* Bookmarked!
