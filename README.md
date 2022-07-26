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

## High SEO & performance score for mobile and web:
[Google PageSpeed Insights](https://developers.google.com/speed/pagespeed/insights/) is without a doubt a useful tool for webmasters, developers, and site owners of all types. However, people spend hours obsessing over optimizing their sites, in order to try and score 100/100 on this test.

The truth is that this isn’t how Google PageSpeed is meant to be used for,nor is it a worthwhile pursuit.

The most important aspect of PageSpeed are the recommendations.The more we focus on the recommendations the better is for our site.

While we should certainly try to improve the page loading time as much as possible, getting a 100/100 in Google PageSpeed isn’t actually that important.

Along with Google PageSpeed there are other platforms such GTmetrix, WebPage Test, PingDom, etc which can help us determine the page performance. However chances are the scores across all these platforms won’t match exactly, which tells us how confusing these numbers can be.What really matters is the actual speed of your website. To put it into perspective,there are sites with average loading times of under 500 milliseconds (which is extremely fast!) that don’t have a 100/100 score on PageSpeed Insights.

### Conclusion
The real purpose of testing the site’s performance with Google PageSpeed Insights isn’t to achieve a high score. Instead, it’s to find problem spots on the site, so that we can optimize them and decrease both the actual and perceived loading times.

## Content Editing Tool for Marketing Team - CMS

Since we will be creating the frontend of the site using Next.js, the content editing side of things would be done using a [headless CMS](https://www.enginess.io/insights/pros-cons-headless-cms) approach.
The iion.io website might have the following pages, each with different data requirements.

-   About Us: This page shows the company information, which will be written directly in the source code. No need to fetch the data
    
-   Blogs: This page shows the list of all blog posts. The data will be fetched from an API.
    
-   Individual Page: This page shows each individual blog page. Similar to blogs page, the data will be fetched from an API.
    
-   Homepage: This page will show the main information about the site. It can contain dynamic as well as static content. Some content will be written directly in the source code while some will be fetched from an API or multiple APIs.
    
One of the best features of Next.js is per page configuration for pre-rendering. We get to choose a different data fetching method for each page.

### Conclusion

While a content editing tool will not allow the marketing team to edit and update the content on all pages. It will still be useful to modify the content on different pages which fetches the data from an external source. Currently there are 4 best React based CMS available: [Sanity Studio](https://www.sanity.io/studio), [Netlify CMS](https://www.netlifycms.org/), [Strapi](https://strapi.io/), and [Graph CMS](https://hygraph.com/nextjs-cms).

  
Note: [Graph CMS(hygraph)](https://hygraph.com/nextjs-cms) is considered to be one of the better choices for a React based application.

## Site Management and Monitoring Service:
### Amazon CloudWatch [paid] - [Link](https://aws.amazon.com/cloudwatch/)
It helps collect and access all the performance and operational data in form logs and metrics from a single platform rather than monitoring them in silos(server, network, databases). It also helps in monitoring the complete stack (applications, infrastructure, and services).
####  Features:

-   Easily collect and store logs
    
-   High resolutions alarms
    
-   Application Insights
    
-   Lambda monitoring insights
    
-   Improve operational performance and resource optimization
    
***Important**: Sometimes live metrics show older data and take time to refresh. It fills the dashboard with stale data.

### Uptime Robot [free + paid] - [Link](https://uptimerobot.com/)
It is probably the best monitoring tool that we can find if we are only looking for a tool that alerts us whenever the site is down. It focuses on performing synthetic checks on the site and APIs every five minutes and provides alerts through a number of integrations with tools like Slack,Telegram and VictorOps.

####  Features:

-   Simple set up process
    
-   Monitors CRON Jobs
    
-   SMS and email notifications are available
    
-   Advanced notifications notifies certain prerequisites for the alerts: Eg: x errors in y minutes
    

  
***Important**: It does not provide real user monitoring and lacks certain features like page insights.

### Pingdom [paid] - [Link](https://www.pingdom.com/)
Pingdom offers a wide range of capabilities, including SSL certificate monitoring and website performance monitoring.With Its user friendly interface it allows real user monitoring solutions that track real time visits to the site and allows the site owner to enhance the site’s performance with data collected from actual people.
Geographical performance is being monitored as well to ensure that your site will have the best possible performance regardless of where the users are accessing it from.

#### Features:

-   Detailed interfaces with user friendly features
    
-   Fast alerting system
    
-   Real user monitoring and synthetic monitoring(simulation monitoring)
    
-   SMS and email notifications are available
    

 ***Important:** It will alert every time a service or third party service goes down but there are sometimes inconsistencies with the alerting system reported by its previous users.
## Unit Testing:
There are three ways to test a Javascript web app. Apart from integration testing and user interface testing, the most important of all is unit testing. With unit testing, we can run independent tests on each functionality.

 For example: we have to provide an input that’s supposed to produce a known output. And if the output that comes after testing matches the known output, then the testing is successful.
Following are some of the most popular Javascript unit testing frameworks:

  

1.  Jest - [Link](https://jestjs.io/): It was the most popular Javascript unit testing framework in 2020. It is a preferred framework for React based applications. It is widely used because it is easy to learn, requires zero setup and manages
    
2.  Cypress - [Link](https://www.cypress.io/)  : This framework runs on a browser, where it provides an interactive interface. It can be used on MAC, Windows and Linuxs. It comes with a test runner which allows automated screenshot and video capturing. It is highly preferred by React Developers.
    

3. StoryBook - [Link](https://storybook.js.org/): This framework makes unit testing easier by helping developers create independent components.Not only is it great for unit testing but it also helps developers document test cases and guidelines.The documents can help other developers who will work on the same projects.

## Automated Testing(Visual):
### BrowserStack - [Link](https://www.browserstack.com/)
It is a cloud based testing tool. Developers and testers can do cross-browser testing of various web applications in different browsers.

  

***Cross Browser testing**: it is a functional testing done to check if the application is working as expected or not in different browsers for different operating systems.

  We can use BrowserStack as a remote lab and can use it as a real desktop browser. It gives us Javascript unit tests and supports over 750 configurations.
## User Acceptance Testing(UAT):
User acceptance testing is a type of testing performed by the end user or the client to verify/accept the software system before moving the software application to the production environment. UAT is done in the final phase of testing after functional, integration and system testing is done.

 ### Purpose:
The main purpose of UAT is to validate end to end business flow. It does not focus on cosmetic errors, spelling mistakes or system testing. UAT is carried out in a separate testing environment with production like set up.

###  Need:
Need of UAT arises once the website has undergone Unit, Integration and System testing because developers might have built the site based on requirements documents by their own understanding and further required changes during development may not be effectively communicated to them. UAT is essential since the requirements may change during the course of development that may not be effectively communicated to the development team.

### Prerequisites:
-   Business Requirements must be available
    
-   Code should be fully developed
    
-   Unit Testing, Integration Testing & System Testing should be completed
    
-   All the reported bugs/issue must be fixed before UAT

### Best Practices: 
Following points should be considered to make UAT successful:

-   Prepare UAT plan early in the project life cycle
    
-   Prepare checklist before the UAT starts
    
-   Set the expectation and define the scope of UAT clearly
    
-   Test end to end business flow and avoid system tools
    
-   Test the system or application with real world scenarios and data
    
-   Conduct feedback session and meeting before moving to production

## Web Based Demo:
Web animation can be used to visualize the various steps in a complex process or idea, to illustrate a simple marketing message, or to move things on a web page is natural to draw attention to something.

It can engage and hold people’s attention longer than a static web page and communicates an idea or concept more clearly and effectively.

Web animation should be smooth, meaningful and support the visitor’s journey. The web designer/animator needs to be aware of how animation fits into the user experience(UX).From a logical point of view, we can divide web animation into two basic types:

1.  A static, non interactive web animation, for example: - GIF
    
2.  A dynamic web animation with user engagement

## Heatmap Tool:
Heatmap tool offers a two dimensional representation of how customers are interacting with a website. When a web page is clicked, hovered over, or scrolled through, the heatmap uses visualization to display this behavior. Typically it overlay dark colors on a webpage to indicate a high usage area versus lighter colors for a low usage area.
###  Must have features:
-   Behavioral Analytics: This features collects and tracks all mouse movements and any user feedback
    
-   Predictive Analysis: AI tools predict future behavior by using data mining and machine learning to identify risk and ROI opportunities that will increase the productivity of a business site.
    
-   Funnel Analysis: Maps a user’s journey through a website and identifies the location where visitors stopped.
    
-   Deployable on Mobile: Can offer deeper insights into mobile experience for users.
    

- Real-time monitoring: Tracks how visitors are using the website in real time

  

## A/B Testing:
A/B testing(also known as split testing) is a method of comparing two versions of a website and app against each other to determine which one performs better. It can be used to continually improve a given experience or improve a single goal like conversion rate over time.

### Process:
-   Collect data: This analytics will often provide information where we can begin optimizing. It provides a way to look for pages with low conversion rates or high drop off rates.
    
-   Identify goals: Goals can be anything from clicking a button or link to email -signups.
    
-   Generate Hypothesis: Once a goal has been identified, we can begin generating A/B testing ideas for why we think they will be better than the current version.
    
-   Create Variations: Make the desired changes to an element of the website or mobile app experience. This might be changing the colour of a button, swapping the order of elements on the page, hiding navigation elements, or something entirely custom.
    
-   Run experiment: kick start the testing and wait for visitors to participate. At this point, visitors will be randomly assigned to different variations of the site. Their interaction with each experience is measured, counted and compared to determine how each performs
    
-   Analyze Results: Once the experiment is complete, results will be analyzed.

### Top A/B testing tool:
1.  #### [Google Optimize](https://marketingplatform.google.com/about/optimize/)
    
2.  #### [Optimizely](https://www.optimizely.com/)
    
3.  #### [Zoho PageSense](https://www.zoho.com/pagesense/)
    
4.  #### [HubSpot](https://www.ventureharbour.com/recommends/hubspot/)
    
5.  #### [Omniconvert](https://www.omniconvert.com/)
### Contact Forms
Forms are an essential part of any business. Whether we are looking for new leads, or want to collect information from our website visitors, forms can be a powerful tool in our marketing arsenal.

  

However not all forms are created equal - some may need to offer more features than others.

We have got two choices either to build forms using a form builder(like Zoho Forms) or build them on our own.

