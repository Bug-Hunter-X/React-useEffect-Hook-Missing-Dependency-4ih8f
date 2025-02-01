# React useEffect Hook Missing Dependency
This repository demonstrates a common error in React applications involving the `useEffect` hook: omitting necessary dependencies from the dependency array.  This can lead to unexpected re-renders, performance issues, and incorrect application behavior. 

The `bug.js` file contains the buggy code, illustrating the missing dependency. The `bugSolution.js` file demonstrates the correct implementation.

## Problem
When a component renders, it's crucial that `useEffect` only runs when its dependencies change. Missing a dependency results in the effect running on every render, causing potential issues such as infinite loops if the effect modifies something within the component.