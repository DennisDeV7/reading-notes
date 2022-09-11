# React 3

## Next JS

[nextjs.org](https://nextjs.org/learn/basics/assets-metadata-css/styling-tips)

Next JS allows for more adaptive implementation of images using an image component. This component also allows for quick build and rendering times as it only loads the images as they enter the viewport on the screen.

Example of a basic image component:

```js
import Image from 'next/image';

const YourComponent = () => (
  <Image
    src="/images/profile.jpg" // Route of the image file
    height={144} // Desired size with correct aspect ratio
    width={144} // Desired size with correct aspect ratio
    alt="Your Name"
  />
);
```

Next also allows for importing third party JavaScript scripts through a Script component. This feature can be used in regular HTML, however, the next component allows for more predictable fetching of the script so you know where it will be rendered.

```js
import Script from 'next/script';

export default function FirstPost() {
  return (
    <>
      <Head>
        <title>First Post</title>
      </Head>
      <Script
        src="https://connect.facebook.net/en_US/sdk.js"
        strategy="lazyOnload"
        onLoad={() =>
          console.log(`script loaded correctly, window.FB has been populated`)
        }
      />
      <h1>First Post</h1>
      <h2>
        <Link href="/">
          <a>Back to home</a>
        </Link>
      </h2>
    </>
  );
}
```

## React Context for Beginners

[freecodecamp.org](https://www.freecodecamp.org/news/react-context-for-beginners/)

React context allows for a developer to pass data to components without the use of props. You can use react context by creating a createContext method and then access it in any component using the context consumer.

Example: 

```js
import React from 'react';

export const UserContext = React.createContext();

export default function App() {
  return (
    <UserContext.Provider value="Reed">
      <User />
    </UserContext.Provider>
  )
}

function User() {
  return (
    <UserContext.Consumer>
      {value => <h1>{value}</h1>} 
      {/* prints: Reed */}
    </UserContext.Consumer>
  )
}
```

## Using Next.js in 2020

Reace is the most popular way to build a website as of 2020. Next.js gives flexibility to render from the server or from the front end depending on the data fetching needs.

Next.JS helps optimize performance automatically. In specific, the page based routing allows the site to only render the code that is relative to that specific route.

Next.JS is built on top of webpack and makes it very user friendly for developers. It allows the react state to preserve through the app. In addition, it has great debugging properties that are not native to JavaScript. It also has great native acceptance for styling methods.

Deploying Next.JS is easy and is commonly done from Vercel. However, it does not have to exclusively be deployed from Vercel.

Community: there are five main developers at Next.JS and they work with or are from major companies such as Facebook and Google.

## Things I want to learn more about