# React Router v6 Catch-all Route Issue

This repository demonstrates a subtle issue with the catch-all route (`/*`) in React Router v6 when used in conjunction with nested routes. The catch-all route unexpectedly intercepts all routes defined after it, regardless of their path. 

The `App.js` file contains the problematic code, while `AppSolution.js` demonstrates a solution.

## Problem

The issue arises because the `/*` route is too general and matches every possible path.  This prevents any subsequent routes from being matched. 

## Solution

The solution involves using more specific routes or ordering routes more strategically.  The solution provided restructures the order of routes to handle more specific paths before the catch-all.  This ensures that only unmatched routes are handled by the catch-all route.