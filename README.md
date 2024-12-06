# React useEffect Hook Unexpected Behavior

This repository demonstrates a common issue encountered when using the `useEffect` hook in React: the effect running on every render despite specifying a dependency array.  The problem is rooted in a misunderstanding of how `useEffect` works with state updates.

The `bug.js` file showcases the problematic code. The `useEffect` hook logs the current `count` to the console on every render, causing an infinite loop.  

The solution provided in `bugSolution.js` addresses the issue by introducing a more efficient approach to updating state within useEffect and making sure that the dependency array is properly set up and used.  

## How to Reproduce

1. Clone the repository.
2. Run `npm install` to install dependencies.
3. Run `npm start` to start the development server.
4. Observe the console output to see the unexpected behavior.

## Solution

The solution uses the updated count value correctly, preventing the infinite render loop and ensuring efficient execution of the effect.