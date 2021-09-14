# Create a Next.js App

- To build a complete web application with React from scratch, there are many important details you need to consider:

- Code has to be bundled using a bundler like webpack and transformed using a compiler like Babel.
  You need to do production optimizations such as code splitting.
  You might want to statically pre-render some pages for performance and SEO. You might also want to use server-side rendering or client-side rendering.
  You might have to write some server-side code to connect your React app to your data store.
  A framework can solve these problems. But such a framework must have the right level of abstraction — otherwise it won’t be very useful. It also needs to have great "Developer Experience", ensuring you and your team have an amazing experience while writing code.

<img src="https://miro.medium.com/max/966/1*OA9c8CovXaqjwbzi_qYKsA.jpeg" width="900px" height="400px">

## Next.js: The React Framework

Enter Next.js, the React Framework. Next.js provides a solution to all of the above problems. But more importantly, it puts you and your team in the pit of success when building React applications.

- Next.js has the best-in-class "Developer Experience" and many built-in features; a sample of them are:

An intuitive page-based routing system (with support for dynamic routes)
Pre-rendering, both static generation (SSG) and server-side rendering (SSR) are supported on a per-page basis
Automatic code splitting for faster page loads
Client-side routing with optimized prefetching
Built-in CSS and Sass support, and support for any CSS-in-JS library
Development environment with Fast Refresh support
API routes to build API endpoints with Serverless Functions

## Fully extendable

Next.js is used in tens of thousands of production-facing websites and web applications, including many of the world's largest brands.

This tutorial assumes basic knowledge of JavaScript and React. If you’ve never written React code, you should go through the official React tutorial first.

If you’re looking for documentation instead, visit the Next.js documentation.

## Editing the Page

Make sure the Next.js development server is still running.
Open pages/index.js with your text editor.
Find the text that says “Welcome to” under the tag and change it to “Learn”.
Save the file.