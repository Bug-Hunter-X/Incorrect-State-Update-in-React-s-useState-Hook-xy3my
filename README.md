# Incorrect State Update in React's useState Hook

This example demonstrates a common mistake when using React's `useState` hook: directly modifying the state variable instead of using the setter function. This can lead to unpredictable behavior and prevent the component from re-rendering correctly.

## Bug
The `bug.js` file contains a component that attempts to increment the state variable `count` directly within a `useEffect` hook.  This bypasses React's state management mechanism, resulting in no visual update of the count.

## Solution
The `bugSolution.js` file shows the correct way to update the state variable using the `setCount` function.  This ensures React properly updates the UI and triggers a re-render of the component.