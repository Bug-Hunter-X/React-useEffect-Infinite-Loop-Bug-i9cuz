# React useEffect Infinite Loop Bug
This repository demonstrates a common bug in React applications involving the `useEffect` hook.  The bug is caused by an incorrectly defined dependency array, leading to an infinite loop.

## Bug Description
The original code attempts to log the current count after every render. However, because the `count` variable is not included in the dependency array, the effect runs after every render, resulting in an infinite loop of updates and re-renders.

## Solution
Adding the `count` variable to the dependency array fixes the bug.  Now, the effect only runs whenever the `count` value changes.
