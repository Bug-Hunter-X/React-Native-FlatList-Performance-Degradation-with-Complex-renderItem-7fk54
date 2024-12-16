# React Native FlatList Performance Bug

This repository demonstrates a common performance issue encountered when using `FlatList` in React Native with large datasets and complex `renderItem` functions. The bug manifests as significant lag and potential crashes, particularly on lower-end devices.

## Problem

The provided `bug.js` file showcases a `FlatList` implementation where the `renderItem` function performs computationally expensive operations for each item, leading to performance bottlenecks.  This results in noticeable UI freezes and a poor user experience.

## Solution

The `bugSolution.js` file presents a solution that addresses the performance problem. This involves several optimization techniques including memoization to reduce redundant calculations and virtualization to render only the visible items in the list, significantly improving performance.

## How to reproduce

1. Clone this repository.
2. Navigate to the project directory.
3. Run `npm install` to install the dependencies.
4. Run `npx react-native run-android` or `npx react-native run-ios` to run the app.
5. Observe the performance difference between `bug.js` and `bugSolution.js`.