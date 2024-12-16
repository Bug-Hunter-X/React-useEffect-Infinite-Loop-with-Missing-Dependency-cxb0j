# React useEffect Infinite Loop Bug

This repository demonstrates a common bug in React's `useEffect` hook: an infinite loop caused by a missing dependency in the dependency array.

## Bug Description
The `MyComponent` component uses `useEffect` to increment a counter every second. However, the dependency array is empty (`[]`), meaning the effect runs only once after the initial render. The interval ID is never cleared, resulting in an infinite loop and causing the counter to update indefinitely.