# Next.js Counter Component Not Updating

This repository demonstrates a common issue in Next.js applications where a counter component fails to update its state after a button click. The issue arises from incorrect state management or missing key dependencies.

## Bug Description

A simple counter component, integrated into a Next.js application, does not update the counter value. Clicking the button does not increment the counter, even though the click event is correctly triggered.

## Reproduction Steps

1. Clone this repository.
2. Navigate to the project directory: `cd nextjs-counter-bug`
3. Install dependencies: `npm install`
4. Run the development server: `npm run dev`
5. Observe that clicking the button has no effect on the counter value.

## Solution

The solution involves ensuring that the component re-renders whenever the state changes. In this case, it was necessary to properly use `useState` hook.