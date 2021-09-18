## How to Statically Generate Pages with Dynamic Routes

In our case, we want to create dynamic routes for blog posts:

We want each post to have the path /posts/<id>, where <id> is the name of the markdown file under the top-level posts directory.
Since we have ssg-ssr.md and pre-rendering.md, we’d like the paths to be /posts/ssg-ssr and /posts/pre-rendering.

## Overview of the Steps

We can do this by taking the following steps. You don’t have to make these changes yet — we’ll do it all on the next page.

- First, we’ll create a page called [id].js under pages/posts. Pages that begin with [ and end with ] are dynamic routes in Next.js.

In pages/posts/[id].js, we’ll write code that will render a post page — just like other pages we’ve created.

- Now, here’s what’s new: We’ll export an async function called getStaticPaths from this page. In this function, we need to return a list of possible values for id.

- Finally, we need to implement getStaticProps again - this time, to fetch necessary data for the blog post with a given id. getStaticProps is given params, which contains id (because the file name is [id].js).

![routes](https://nextjs.org/static/images/learn/dynamic-routes/how-to-dynamic-routes.png)

## Implement getStaticPaths

- First, let’s set up the files:

Create a file called [id].js inside the pages/posts directory.
Also, remove first-post.js inside the pages/posts directory — we’ll no longer use this.
Then, open pages/posts/[id].js in your editor and paste the following code. We’ll fill in ... later

- Then, open lib/posts.js and add the following getAllPostIds function at the bottom. It will return the list of file names (excluding .md) in the posts directory

- Finally, we'll import the getAllPostIds function and use it inside getStaticPaths. Open pages/posts/[id].js and copy the following code above the exported Post component