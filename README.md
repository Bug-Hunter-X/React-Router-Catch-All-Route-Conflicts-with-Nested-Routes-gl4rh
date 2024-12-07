# React Router Catch-All Route Conflict

This repository demonstrates a common issue in React Router v6 where a catch-all route (`*`) conflicts with other routes, leading to unexpected rendering or navigation issues.  The problem arises when the catch-all route is positioned incorrectly, unintentionally intercepting navigation intended for other routes.

## Problem

The provided `App.js` demonstrates a scenario where a nested route is incorrectly handled due to the catch-all route's placement.  Navigation to intended routes fails as the catch-all route intercepts the request.

## Solution

`AppSolution.js` presents a corrected version where route order is carefully managed to avoid conflicts. The catch-all route is placed after the specific routes to ensure that it only handles requests not matched by more specific routes.