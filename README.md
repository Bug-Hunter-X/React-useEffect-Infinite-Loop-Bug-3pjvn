# React useEffect Infinite Loop Bug

This repository demonstrates a common bug in React applications involving the `useEffect` hook and how to fix it.

## Bug Description

Forgetting to include a dependency array in `useEffect` can lead to an infinite loop, causing performance issues and potentially crashing the application.  The infinite loop occurs because the effect runs after every render, triggering a re-render, which in turn triggers the effect again.

## Bug Solution

The solution involves correctly specifying the dependency array to ensure the effect only runs when the dependencies change.

## How to reproduce

1. Clone the repository
2. Run `npm install`
3. Run `npm start`
4. Observe the console and the counter behavior in the bug.js example.
5. Compare it with the correct implementation in bugSolution.js

## Additional Resources

* [React documentation on useEffect](https://reactjs.org/docs/hooks-reference.html#useeffect)