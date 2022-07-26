# iion.io - Tech Specification

## Tech Stack:
###  Next JS
Next.js is a React framework that supports pre-rendering. Instead of having the browser render everything from scratch, Next.js can serve pre-rendered HTML in two different ways
With Server-side Rendering (SSR), Next.js pre-renders the page into HTML on the server on every request which makes sure the data is always up to date.

With Static Generation (SSG), Next.js pre-renders the page into HTML on the server ahead of each request, such as at build time. The HTML can be globally cached by a CDN and served instantly.SSG is more performant, but because pre-rendering happens ahead of time, the data could become stale at request time.

Fortunately, with Next.js - SSG can be used for maximum performance without sacrificing the benefits of Server Side Rendering.


### SASS/SCSS - Custom Styling

Sass is the most mature, stable, and powerful professional grade CSS extension language in the world.

CSS itself has given us native solutions to some of the problems SASS originally solved and we’ve got so many options for development these days with Styled Components in React, Tailwind, CSS-in-JS etc.

However, SASS will not lose its relevance any time soon. Recent CSS features are cool but using them is cumbersome compared to what SASS has. And compiling scss to generate a so-called CSS4 file is best of both worlds.

####  Benefits:

-   CSS Compatible
    
-   Feature Rich
    
-   Industry Approved
    
-   Large Community

###  AntDesign
An enterprise-class UI design language and React implementation with a set of high-quality React components, one of best React UI libraries for enterprises.

It is easy to use, and mobile-friendly. It supports any major mobile browser, including IE9+. There are components for every screen size and they’re optimized to load only what you need. While it’s more flexible than Bootstrap or Foundation, it doesn’t have as many components or as much code written for them—it’s an open-source project so any developer can contribute to it.

### MongoDB
We all know that in the database technology world, it comes down to two main database types — SQL (relational) and NoSQL (non-relational). The differences between them are rooted in the way they are designed, which data types they support, and how they store them.

Our preferred choice of database is a NoSQL one. NoSQL commonly referred to as “Not Only SQL”. With NoSQL, unstructured, schema less data can be stored in multiple collections and nodes and it does not require fixed table sachems, it supports limited join queries, and we scale it horizontally.

#### Benefits of NoSQL database:

-   HIghly and easily scalable
    
-   Maintaining NoSQL servers are less expensive
    
-   No Schema or Fixed Data model
    
-   Support Integrating Caching
