# Firebase Asynchronous Operation Error: Accessing Document Snapshot Before Promise Resolution

This repository demonstrates a common error encountered when working with Firebase's asynchronous operations and provides a solution.

## Problem
When using Firebase's `get()` method to fetch data from Firestore, the operation is asynchronous.  Attempting to access properties of the returned `DocumentSnapshot` before the promise resolves leads to undefined values or errors.

## Solution
The solution involves using `.then()` to handle the promise's resolution and access the data only after the promise is fulfilled. Error handling is also implemented to manage potential issues during the data retrieval process.

## How to reproduce the bug
1. Clone the repository.
2. Run `npm install` to install the required packages.
3. Run `node bug.js` to see the error. 
4. Run `node bugSolution.js` to see the solution.
