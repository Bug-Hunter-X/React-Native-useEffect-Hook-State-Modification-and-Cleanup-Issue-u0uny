# React Native useEffect Hook State Modification and Cleanup

This repository demonstrates a common error in React Native applications related to the `useEffect` hook: incorrectly modifying state and neglecting cleanup.

The `bug.js` file showcases the problematic code, while `bugSolution.js` provides the corrected version.

The error arises from directly manipulating the state variable within the `useEffect` callback and failing to provide a cleanup function to handle side-effects when the component unmounts. This leads to unexpected behavior, including inconsistent rendering and potential memory leaks.

The solution emphasizes using the `setState` function for state updates and providing a return function within the `useEffect` to perform necessary cleanup.