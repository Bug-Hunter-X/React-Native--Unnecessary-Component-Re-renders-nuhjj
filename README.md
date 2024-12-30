# React Native Unnecessary Component Re-renders

This repository demonstrates a common performance issue in React Native applications where components re-render unnecessarily, even though their output remains the same. This is often due to overly broad dependency arrays in `useEffect` hooks or unnecessary state updates.

The `unnecessaryRerenderBug.js` file shows the problematic code, where a component re-renders whenever its `data` prop changes, despite only using the `data.name` property.  The `unnecessaryRerenderSolution.js` demonstrates how to solve this using techniques like `useMemo`, `React.memo`, or by carefully specifying dependencies in `useEffect`. 

This example highlights the importance of optimizing component re-renders for performance in React Native.