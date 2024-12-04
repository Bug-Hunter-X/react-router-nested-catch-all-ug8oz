# React Router Dom v6 Nested Routes and Catch-All Route Issue

This repository demonstrates a bug in React Router Dom v6 related to nested routes and the catch-all route (`/*`). The catch-all route is not working as expected, always showing the Not Found component even when there is a valid path.

## Bug Description

The issue occurs when using nested routes along with a catch-all route to handle 404 errors. Despite having defined routes, the catch-all route (`/*`) is triggered even if other routes match the URL path.

## Solution

The solution involves carefully placing the catch-all route within the parent route to ensure that it's only triggered when no other child routes match.

## How to reproduce

1. Clone this repository.
2. Install the dependencies using `npm install` or `yarn install`.
3. Run `npm start` or `yarn start`.
4. Navigate to different routes to observe the issue.