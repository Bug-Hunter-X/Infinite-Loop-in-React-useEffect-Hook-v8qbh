# React useEffect Infinite Loop Bug

This repository demonstrates a common error in React applications involving the `useEffect` hook.  The example shows an infinite loop caused by updating state within the `useEffect` function without appropriate dependency management.

## Bug Description

The `MyComponent` component uses `useEffect` to update the `count` state. However, it does so without any dependencies, leading to a continuous update cycle and an infinite loop. This causes the browser to crash or become unresponsive.

## Solution

The solution involves properly managing dependencies in the `useEffect` hook.  The corrected component in `bugSolution.js` demonstrates how to fix this by only updating the state when certain values change.