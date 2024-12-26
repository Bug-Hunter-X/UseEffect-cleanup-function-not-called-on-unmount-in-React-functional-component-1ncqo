# React useEffect Cleanup Function Issue

This repository demonstrates a subtle bug related to the cleanup function in React's `useEffect` hook within a functional component.  The issue arises when specific conditions are met concerning component unmounting and the use of the `useState` hook.

## The Problem

The provided `bug.js` file contains a React functional component that utilizes `useEffect` with a cleanup function. Under certain circumstances, this cleanup function isn't consistently called when the component unmounts, leading to potential memory leaks or unexpected behavior.  The specific conditions triggering this inconsistency are explored and resolved in the solution.

## Solution

The solution, found in `bugSolution.js`, addresses the problem by ensuring the cleanup function executes reliably upon unmounting.  The changes made highlight best practices to prevent this type of issue and improve the overall robustness of the code.

## How to Reproduce

1. Clone this repository.
2. Run `npm install` to install dependencies.
3. Run `npm start` to start the development server.
4. Observe the console logs to verify the behavior of the cleanup functions in both `bug.js` and `bugSolution.js` when the component mounts and unmounts.