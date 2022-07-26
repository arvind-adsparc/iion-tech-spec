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

