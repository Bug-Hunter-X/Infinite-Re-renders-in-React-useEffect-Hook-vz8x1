# React useEffect Infinite Loop Bug

This repository demonstrates a common error in React's `useEffect` hook, leading to infinite re-renders.

## Problem

The `useEffect` hook's dependency array is incorrectly configured, causing the effect to run on every render, creating an infinite loop. This usually happens when a state variable used within the effect is not included in the dependency array.

## Solution

The solution involves correctly specifying the dependencies in the `useEffect` hook. By adding the state variable (`count`) to the dependency array, the effect only runs when the value of `count` changes.