# All-About-next-js

✅ What is NEXT JS ?
     Next.js is framework that build on top of React.js that gives you the flexibility of building scalable apps by allowing you to render content on server.

    React JS use client side rendering (CSR) technique only. On the other hand, Next.js provides us three techniques such as: Static site generation, Server side rendering (SSR), Incremental Site generation.

✅ What is Client Side Rendering (CSR)?
    ➡️ CSR is a rendering technique where only the html skeleton is rendered on the server and the complete page render happening on the browser (client side) by downloading and executing all the necessary JavaScript.

    ➡️ Advantage of CSR: 
        1. Reduced Server Load: The server only needs to provide the initial HTML and JavaScript files, leading to lower server-side rendering overhead.
        2. Simplified Backend Logic: With CSR, the server primarily acts as a data API, leading to a cleaner and simpler backend codebase.

    ➡️ Limitations of CSR: 
        1. Slower Initial Page Load: CSR can result in a slower initial page load as the browser needs to download and execute JavaScript before rendering the page.
        2. SEO Challenges: Search engines may not effectively crawl or index content generated dynamically through JavaScript, potentially affecting SEO and discoverability.

✅ What is Static Site Generation (SSG)?
    ➡️ SSG is a web development technique that pre-generates HTML files for web pages during the build or deployment process. This allows the server to immediately deliver the static HTML to a user's browser when they visit a page, without needing to do any extra work. SSG is a good approach for websites with content that doesn't change often, like blogs or documentation.

✅ What is Server Side Rendering (SSR)?
    ➡️ SSR is the process of rendering the complete HTML page form the server to the client by collecting and combining data from the cloud in response to a request and returning it to the client.

    ➡️ Advantages of SSR:
        1. Faster Initial Page Load Time: SSR significantly reduces the initial page load time as the client receives pre-rendered content from the server, resulting in a faster perceived load time.
        2. SEO Benefits: Search engines can easily crawl and index content since the complete HTML is available in the initial response. This improves the discoverability and ranking of your web pages.
        3. Better Performance on Low-End Devices: SSR is advantageous for users on low-end devices or slow internet connections since most of the rendering process is handled by the server.

    ➡️ Limitations of SSR:
        1. Increased Server Load: SSR can put a considerable load on the server, especially when dealing with a large number of simultaneous requests, impacting server response times.
        2. Reduced Interactivity: As most rendering happens on the server-side, interactions within the application may be slower compared to CSR, as additional requests may be needed to update the page content.

✅ What is Incremental Static Regeneration (ISR)?
    ➡️ ISR is a combination of SSG and SSR that allows updating of existing pages and adding new ones, by pre-rendering a subset of pages in the background even while receiving new requests for pages.