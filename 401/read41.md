# React 4

## Dynamic Routes

Next.js enables a developer to statically generate pages with paths that depend on external data. In order to make a dynamic page you must follow these steps:

1. create a page with with a name in brackets such as: [id].js
2. Inside the file you will need a react component to render the page
3. getStaticPaths which returns an array of possible values for id
4. getStaticProps which fetches necessary data for the post with id

## Deployment

1. Create an account on Vercel
2. import your project to vercel
3. use default value for deploy settings
4. preview
5. deploy

Next.js came up with their own method for the workflow which they call DPS (Develop, Preview, Ship).

Next.js projects can be deployed from any provider that supports Node.js.

## Things I want to learn more about