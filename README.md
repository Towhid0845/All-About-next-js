# All-About-next-js
In this document, we will about learn next.js and implement it in a project. You need to have basic concept of react js to start.
### What is NEXT JS ?
Next.js is framework that build on top of React.js that gives you the flexibility of building scalable apps by allowing you to render content on server.

**React JS use client side rendering (CSR) technique only. On the other hand, Next.js provides us three techniques such as: Static site generation, Server side rendering (SSR), Incremental Site generation.**

#### What is Client Side Rendering (CSR)?
CSR is a rendering technique where only the html skeleton is rendered on the server and the complete page render happening on the browser (client side) by downloading and executing all the necessary JavaScript.

➡️ Advantage of CSR: 
* Reduced Server Load: The server only needs to provide the initial HTML and JavaScript files, leading to lower server-side rendering overhead.
* Simplified Backend Logic: With CSR, the server primarily acts as a data API, leading to a cleaner and simpler backend codebase.

➡️ Limitations of CSR: 
* Slower Initial Page Load: CSR can result in a slower initial page load as the browser needs to download and execute JavaScript before rendering the page.
* SEO Challenges: Search engines may not effectively crawl or index content generated dynamically through JavaScript, potentially affecting SEO and discoverability.

#### What is Static Site Generation (SSG)?
SSG is a web development technique that pre-generates HTML files for web pages during the build or deployment process. This allows the server to immediately deliver the static HTML to a user's browser when they visit a page, without needing to do any extra work. SSG is a good approach for websites with content that doesn't change often, like blogs or documentation.

#### What is Server Side Rendering (SSR)?
SSR is the process of rendering the complete HTML page form the server to the client by collecting and combining data from the cloud in response to a request and returning it to the client.

➡️ Advantages of SSR:
* Faster Initial Page Load Time: SSR significantly reduces the initial page load time as the client receives pre-rendered content from the server, resulting in a faster perceived load time.
* SEO Benefits: Search engines can easily crawl and index content since the complete HTML is available in the initial response. This improves the discoverability and ranking of your web pages.
* Better Performance on Low-End Devices: SSR is advantageous for users on low-end devices or slow internet connections since most of the rendering process is handled by the server.

➡️ Limitations of SSR:
* Increased Server Load: SSR can put a considerable load on the server, especially when dealing with a large number of simultaneous requests, impacting server response times.
* Reduced Interactivity: As most rendering happens on the server-side, interactions within the application may be slower compared to CSR, as additional requests may be needed to update the page content.

#### What is Incremental Static Regeneration (ISR)?
ISR is a combination of SSG and SSR that allows updating of existing pages and adding new ones, by pre-rendering a subset of pages in the background even while receiving new requests for pages.

### Benefit of Next.js
1. **Different Rendering techniques (SSG, SSR, ISR) as discussed before**.
2. **Performance**
    * **Code Splitting:** Divide your web app in small chunks so you can only load the chunk that is used by the current page. ![alt text](image.png) Next.js downloads chunk by chunk which is needed for the page (not entire page).
    * **Minifying Files:** It makes file size very very small that's why the performance gets a huge boost.
    * **Image Optimizations:** It provide us an Next Image Component which optimize images automatically and it sevres according to devices (check it in network tab at browser dev mode).
    * **Prefetching Assets:** Next.js automatically prefetch images according to the view point (when we scroll).
3. **File Base Routing:** Next.js provides premeditated built-in file based routing system (we don't need to install any extra package).
4. **SEO:** It provide extra features like so that SEO can be done smoothly.
5. **Serverless Functions:** All the files under 'api' directory comes with already configured node server. When it needs, it weak up the server and execute the task and automatically shuts it down. We don't need to running the server all the time.

_Now, Let's get started with creating a new next application._

### How to Create a Next App ?
We need to use package manager for creating a next app. We can use 'npm' or 'yarn', both are good. Here we are using npx (It stands for Node Package Execute and is included with npm. It's a npm package runner that can execute any package from the npm). 

    Command to create a next application: 
        npx create-next-app

_If you find any vulnerabilities(high) while installing any package, it should be fixed using `npm audit-fix` command._

***
## Need to Study:
### Next Architecture
### Next Compiler
#### SWC
### Middleware
Whenever a user sends a request, if first goes to the middleware, the code that is sitting in the middleware runs and then the request gets forwarded to the actual code. For example, if there is a middleware sitting between an API call (the request), for that case, middleware will first run and then the API will run.

### Server Component

### Edge Function (vercel)
The closer are server, the faster are responses going to be. It works with middleware. Middleware deploy the codes to the edge function and edge function works as a server. The fact that we are deploying thing to vercel is that, a lot of our middleware code get automatically deployed to edge function. Edge functions essentially help us to understand hey, this specific user has this specific location, should I even run the API code and If it is not needed they are not going to run it. That's the beauty of it ! that's the power of edge function.

### Routing

### video up to 18 done.


