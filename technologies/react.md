# React and Redux

## Basic

1. **What is the difference between a class component and a functional component?**

   - Functional Components: A functional component is just a plain JavaScript pure function that accepts props as an argument and returns a React element(JSX), there is no render method used in functional components, functional component run from top to bottom and once the function is returned it cant be kept alive, also known as Stateless components as they simply accept data and display them in some form, that they are mainly responsible for rendering UI, react lifecycle methods (for example, componentDidMount) cannot be used in functional components, hooks can be easily used in functional components to make them Stateful, constructors are not used.
   - Class Components: A class component requires you to extend from React. Component and create a render function which returns a React element, it must have the render() method returning JSX (which is syntactically similar to HTML), class component is instantiated and different life cycle method is kept alive and being run and invoked depending on phase of class component, also known as Stateful components because they implement logic and state, react lifecycle methods can be used inside class components (for example, componentDidMount), it requires different syntax inside a class component to implement hooks, constructor are used as it needs to store state.

2. **What is a High Order Component?**
   - A higher-order component is a function that takes a component and returns a new component. A higher-order component (HOC) is the advanced technique in React. js for reusing a component logic. Higher-Order Components are not part of the React API. They are the pattern that emerges from React's compositional nature.
3. **What is the difference between state and props?**
   - The key difference between props and state is that state is internal and controlled by the component itself while props are external and controlled by whatever renders the component.
4. **What are CSS Modules?**
   - CSS Module is simply a . css file, where classes act similarly to local variables in Javascript. It is a tool that makes every class unique by including a hash in their name.
5. **What are React Hooks and what problem do they solve?**
   - A Hook is a javascript function that allows to create/access React state and lifecycle and that, in order to ensure the stability of the application. The ultimate purpose of hooks is to simplify the actual logic, React provides only a reduced set, with the flexibility to respond to various situations in the lifecycle of an application and the possibility to build our own as well.
6. **What is React Suspense?**
   - React Suspense is a React component that suspends a component('s) being render until a certain condition has been met, and will display a fallback option. This fallback option is required, and it may be a string or another React component such as a spinner.
7. **What is the difference between Real DOM and Virtual DOM?**
   - A virtual DOM object has the same properties as a real DOM object, but it lacks the real thing's power to directly change what's on the screen. Manipulating the DOM is slow. Manipulating the virtual DOM is much faster, because nothing gets drawn onscreen.
8. **What is "key" prop and what is the benefit of using it in arrays of elements?**
   - A key is a special string attribute you should include when creating arrays of elements. Key prop helps React identify which items have changed, are added, or are removed.
9. **What are fragments?**
   - React Fragments allow you to wrap or group multiple elements without adding an extra node to the DOM. This can be useful when rendering multiple child elements/components in a single parent component.
10. **Could you explain useMemo and useCallback**
    - useCallback: The useCallback hook is used when a child component is rerendering over and over again without any need. By using useCallback, you can prevent unnecessarily re-rendering components by returning the same instance of the function that is passed instead of creating a new one each time.
    - useMemo: The useMemo hook is used in the functional component of React to return a memoized value. In computer science, memoization is a concept used in general when we can save re-compilation time by returning the cached result. In the functional component of React, useMemo hooks provide memory-mapped values. Using useMemo when very little processing is involved is not really wise. In cases with very little processing, using it could add extra overhead. However, useMemo works well to avoid extra rendering unnecessarily.
11. **What testing tools have you used to write unit / E2E tests?**
    - There's no right answer
12. **What’s snapshot testing and what are the benefits of it?**
    - Snapshot testing is a type of “output comparison” or “golden master” testing. These tests prevent regressions by comparing the current characteristics of an application or component with stored “good” values for those characteristics. Snapshot tests are fundamentally different from unit and functional tests. While these types of tests make assertions about the correct behavior of an application, snapshot tests only assert that the output now is the same as the output before; it says nothing about whether the behavior was correct in either case.
