# React Native: Accessing State Before Initialization

This repository demonstrates a common error in React Native: accessing a state variable before it has been initialized.  This usually happens when a state variable is used in the render method before the component has mounted.

The `bug.js` file shows the problematic code that attempts to access the state before it's ready.  The `bugSolution.js` file provides a corrected version.

## How to reproduce

1. Clone the repository.
2. Run `npm install`.
3. Run `npx react-native run-android` or `npx react-native run-ios`.
4. Observe the error (if present) in the bug file.

## Solution

The solution involves using conditional rendering or the optional chaining operator to prevent accessing the state before it's been set by React. 