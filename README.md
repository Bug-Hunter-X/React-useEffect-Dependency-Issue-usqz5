# React useEffect Dependency Issue

This repository demonstrates a common bug in React involving the `useEffect` hook and its dependencies array.  Improperly managing dependencies can lead to infinite render loops or unexpected side effects.

## The Bug

The `bug.js` file contains a component that uses `useEffect` to log the render count. However, it's missing `count` from the dependency array, causing the effect to run on every render, creating an infinite loop and filling the console with logs.

## The Solution

The `bugSolution.js` file corrects the issue by adding `count` to the dependency array. Now, the effect only runs when the `count` value changes, resolving the infinite loop problem. 