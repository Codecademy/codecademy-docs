---
Title: 'What is Server-Side Rendering?'
Description: 'Server-side rendering (SSR) is rendering the content on the server and presenting it to the client when a request is made.'
Subjects:
  - 'Computer Science'
  - 'Web Development'
Tags:
  - 'Web Development'
  - 'Server-Side Rendering'
  - 'Computer Science'
CatalogContent:
  - 'paths/computer-science'
  - 'paths/front-end-engineer-career-path'
---

Server-side rendering (SSR) is rendering the content on the server and presenting it to the client when a request is made. When a request is made in client-side rendering (opposite of server-side rendering), the server sends separate files and content that is rendered in the browser. JavaScript works both on the server and browser, so it is possible for developers to render the content of an application where they want.

## Why Server-Side Rendering is Important

- When content is rendered on a server, the time required for downloading, parsing, and executing JavaScript code is reduced. This will ensure fast load times for web pages.

- SSR helps in improving SEO (Search Engine Optimization) by pre-rendering the page. Thus, search engine crawlers can easily read the generated HTML file. In client-side rendering, crawlers read an empty HTML file with links to JavaScript that reduce the search ranking of the web page. Fast loading of the server-side rendered web page also helps the site rank higher in search results.

- When the user clicks on a link for some content, the whole website is rendered again on the server. And if the number of concurrent users increases, the load on the servers increases. At scale, this can be troubling for SSR.
