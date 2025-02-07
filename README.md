# React useEffect setInterval memory leak
This example demonstrates a common mistake in React when using `setInterval` within the `useEffect` hook without proper cleanup.  The `setInterval` function continues to run even after the component unmounts, leading to memory leaks and potential performance issues.

The solution shows how to correctly use `setInterval` with a cleanup function to prevent this problem.  This cleanup function is crucial for ensuring that the interval is cleared when the component is unmounted.