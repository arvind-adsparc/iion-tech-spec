# iion.io - Tech Specification

## Tech Stack:
###  Next JS
Next.js is a React framework that supports pre-rendering. Instead of having the browser render everything from scratch, Next.js can serve pre-rendered HTML in two different ways
With Server-side Rendering (SSR), Next.js pre-renders the page into HTML on the server on every request which makes sure the data is always up to date.

With Static Generation (SSG), Next.js pre-renders the page into HTML on the server ahead of each request, such as at build time. The HTML can be globally cached by a CDN and served instantly.SSG is more performant, but because pre-rendering happens ahead of time, the data could become stale at request time.

Fortunately, with Next.js - SSG can be used for maximum performance without sacrificing the benefits of Server Side Rendering.
