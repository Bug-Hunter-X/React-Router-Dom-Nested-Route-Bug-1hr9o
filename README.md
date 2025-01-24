# React Router Dom Nested Route Bug

This repository demonstrates a common issue with nested routes in React Router Dom.  The bug arises from an incorrectly configured route structure, leading to problems rendering nested components.

## Bug
The `App` component doesn't include a catch-all route for handling nested routes.  This leads to incorrect routing and potential errors when attempting to access nested pages within a route that doesn't have a defined nested route structure. 

## Solution
The solution involves adding nested routes to handle the different sub-paths of the parent route (e.g., `/about`). This ensures that the React Router correctly matches URLs to the corresponding components.

## How to reproduce
1. Clone this repository.
2. Run `npm install`.
3. Run `npm start`.
4. Navigate to `/` (works)
5. Navigate to `/about` (works)
6. Add a nested route (e.g., `/about/contact`) - will likely result in an error due to the missing nested route handling.
