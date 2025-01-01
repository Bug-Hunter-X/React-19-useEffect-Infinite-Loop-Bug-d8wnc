# React 19 useEffect Infinite Loop Bug

This repository demonstrates a common bug in React 19 involving infinite loops within the `useEffect` hook.  The bug arises from improper usage of the dependency array, leading to the effect running repeatedly and causing performance issues or application crashes.

## Bug Description
The provided `bug.js` file contains a `useEffect` hook that's missing essential dependencies, triggering an infinite loop. Each state update causes the effect to run again, leading to a cascading effect. 

## Solution
The `bugSolution.js` file demonstrates the fix.  By properly including `count` in the dependency array, the effect runs only when the count changes, resolving the infinite loop.

## How to Reproduce
1. Clone the repository
2. Run `npm install`
3. Run `npm start`
4. Observe the infinite loop in the console of `bug.js` and the corrected behavior of `bugSolution.js`