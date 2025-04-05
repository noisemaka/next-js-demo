# Next.js Tutorial Notes

### Project Structure:

- `/app` contains routes, components, and logic.
- `/app/lib` contains utility and data fetching functions as well as type definitions
- `/app/ui` contains UI components and styles
- `/public` contains static assets for the app

### Layouts and Pages

#### Pages

Next.js uses a file-system router where folders are mapped to route segments in the application's URL.

The page.tsx file exports a React component is **required** for the route to be accessible.

Nested routes are creating by nesting folders within one another.

e.g. `/app/dashboard/` will map to url.com/dashboard while `app/dashboard/customers` will map to url.com/dashboard/customers.

#### Layouts

Layout files are used to define UI which is shared among pages. You can create one for each nested route if necessary.

This component recieves a children prop, which can be another page or layout.

On navigation, only the page components will update and the layout will not re-render.

A root layout is **required** for any Next.js application.
