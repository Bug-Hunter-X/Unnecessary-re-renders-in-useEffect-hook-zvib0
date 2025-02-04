# Unnecessary Re-renders in React useEffect Hook

This example demonstrates a common mistake when using the `useEffect` hook in React: forgetting to specify a dependency array or specifying it incorrectly. This can lead to unexpected re-renders and performance issues.

The `bug.js` file shows the problematic code. The `useEffect` hook runs on every render because the dependency array is missing, causing the component to re-render continuously and log to the console repeatedly.

The `bugSolution.js` file provides a corrected version.  The dependency array `[count]` ensures that the effect only runs when the `count` variable changes.