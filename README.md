# Frequently Asked Front End Questions 
 ### Resources 
 

 ## Table of Contents

- [1 What does client-side mean?](#what-does-client-side-mean)
- [2 What is node.js](#what-is-nodejs)
- [3 Is cross browser testing necessary?](#is-cross-browser-testing-necessary)
- [4 Why do we use unit testing?](#why-do-we-use-unit-testing)
- [5 Can you explain about web Accessibility ?](#can-you-explain-about-web-accessibility)
- [6 What are sitemap in SEO?](#what-are-sitemap-in-seo)
- [7 Can you describe some SEO best practices or techniques ?](#can-you-describe-some-seo-best-practices-or-techniques)
- [8 How can we use a multiply stylesheet?](#how-can-we-use-a-multiply-stylesheet)
- [9 How can we improve website’s assets or resources?](#how-can-we-improve-websites-assets-or-resources)
- [10 How many resources will a browser download from a given domain at a time?](#how-many-resources-will-a-browser-download-from-a-given-domain-at-a-time)
- [11 How DOM is rendered?](#how-dom-is-rendered)
- [12 What does server side mean?](#what-does-server-side-mean)
- [13 Where is DOM stored?](#where-is-dom-stored)
- [14 What does headless mean in software?](#what-does-headless-mean-in-software)
- [15 How do I use headless browser?](#how-do-i-use-headless-browser)
- [16 What is WebView used for?](#what-is-webview-used-for)
- [17 What is the difference HTTP and https?](#what-is-the-difference-http-and-https)
- [18 What is TLS (Transport Layer Security)?](#what-is-tls-transport-layer-security)
- [19 What is a network protocol?](#what-is-a-network-protocol)
- [20 What does a CMS actually do?](#what-does-a-cms-actually-do)
<br/><br/><br/><br/>

1. ### What does client-side mean?

In web development, 'client side' refers to everything in a web application that is displayed or takes place on the client (end user device). This includes what the user sees, such as text, images, and the rest of the UI, along with any actions that an application performs within the user's browser.

Markup languages like HTML and CSS are interpreted by the browser on the client side.

2. ### What is node.js

Node.js is an open-source, cross-platform, back-end JavaScript runtime environment that runs on the V8 engine and executes JavaScript code outside a web browser.

3. ### Is cross browser testing necessary?

Different browsers and operating systems have different ways of handling code. The smallest errors, like forgetting a semicolon or not closing a tag, may behave differently in different environments. Some browsers may render the component easily, while others may throw errors or not show anything at all. This can be pointed out with the help of cross-browser testing. Cross-browser testing is also necessary for example in javascript code we have a new feature but old browsers don't support it. this can be also figured out while testing.

4. ### Why do we use unit testing?

Unit test provide a way to test small units of code independently of the larger system. This is useful to check that an application is meeting its requirements, and to ensure that the code is working as expected.

**Benefits of unit testing:**

 1. It is a good way to test small units of code independently of the larger system.
 2. Increases code readability.
 3. improve deployment velocity.

**Examples of Init testing in JS:**

```javascript
const sum = (a, b) => a + b;
describe('sum', () => {
  it('should add two numbers', () => {
    expect(sum(1, 2)).toBe(3);
  });
}
```

5. ### Can you explain about web Accessibility ?

Accessibility is also known as the ability of access, Web accessibility Is the ability of a user to use a web page, web application, or web service with their disabilities. In Example In HTML we use an image tag to display an image also we have an alt attribute in the image tag Which is used to display the image in case of the image is not found. This can be useful for people with disabilities to understand the content of the page. using their visual impairments devices.

6. ### What are sitemap in SEO?

A sitemap provides information about the structure of your website. You’ll mostly use them to help crawlers and users navigate your site.

Sitemaps are available in XML (eXtensible Mark-up Language) or HTML format. XML files share important information about your website — like its internal links, backlinks, and page structure — in a language search engine crawlers understand.

These search engine crawlers (like Google’s bots) consider this data when deciding your website’s page authority and ranking on their SERPs.

7. ### Can you describe some SEO best practices or techniques ?

- **Meta Descriptions**: A meta description is a brief summary of a page in the SERP (search engine results page) displayed below the title tag.

- **Optimize Images**: Image are considered as important for the search engine to index. When an image is optimized, it is reduced in size of the page load time and image alt text is also most important for the search engine to index.

- **Internal Linking Structure**: Internal links are important because they establish an information hierarchy for your website and also help Google get a deeper understanding of the content on your page

8. ### How can we use a multiply stylesheet?

Handling multiple stylesheets is a common problem in web development. The solution is to use a single stylesheet that contains all of the rules for the different stylesheets. This can be done by combining all of the stylesheets into one stylesheet using a bundler like [Bower](http://bower.io/). or [Gulp](http://gulpjs.com/). Also, we can use the `@import` directive to import the stylesheets.

```css
@import "reset";
@import "base";
@import "layout";
@import "typography";
```

9. ### How can we improve website’s assets or resources?

their are various ways to optimize the website assets.

1. Use CDN(Content Delivery Network)
2. Host website on Edge server.
3. Minimize the number of JavaScript and CSS files
4. Optimize the size of images.
5. Use website caching.
6. Reduce redirects.
7. Use prefetching techniques

10. ### How many resources will a browser download from a given domain at a time?

It depends on the browser and how it is setup - firefox has controls for how many download threads to use, for example.
The different browsers (and versions) have different defaults as well.

IE7 allowed only two concurrent connections per host. But most browsers today allow more than that. IE8 allows 6 concurrent connections, Chrome allows 6, and Firefox allows 8.

11. ### How DOM is rendered?

When a web page is loaded, the browser first reads the HTML text and constructs DOM Tree from it. Then it processes the CSS whether that is inline, embedded, or external CSS and constructs the CSSOM Tree from it. After these trees are constructed, then it constructs the Render-Tree from it. A Render-Tree is a tree of Render-Nodes that represents the final output of the page.

12. ### What does server side mean?

`server side` means everything that happens on the server, instead of on the client. In the past, nearly all business logic ran on the server side, and this included rendering dynamic webpages, interacting with databases, identity authentication, and push notifications.

13. ### Where is DOM stored?

DOM (Document Object Model) is a Tree representation of the page, starting from the <html> tag, going down into every child, which are called nodes. It's kept in the browser memory, and directly linked to what you see in a page.

14. ### What does headless mean in software?

Headless software (e.g. "headless browser" or "headless Linux",) is software capable of working on a device without a graphical user interface. Such software receives inputs and provides output through other interfaces like network or serial port and is common on servers and embedded devices.

15. ### How do I use headless browser?

Headless browsers are a web browser without a graphical user interface that can be controlled from a command line interface programmatically for the purpose of web page automation (e.g., functional testing, scraping, unit testing, etc.). Think of headless browsers as a browser that you can run programmatically from the command line that can retrieve and traverse web page code.

The most common headless browsers are:

- Headless Chromium
- Puppeteer

16. ### What is WebView used for?

Webviews are used by a native OS, in a native application, to run web pages. Think of a webview like an iframe or a single tab from a web browser that is embedded in a native application running on a device (e.g., iOS, android, windows).

17. ### What is the difference HTTP and https?

HTTPS is HTTP with encryption and verification. The only difference between the two protocols is that HTTPS uses TLS (SSL) to encrypt normal HTTP requests and responses, and to digitally sign those requests and responses. As a result, HTTPS is far more secure than HTTP.

18. ### What is TLS (Transport Layer Security)?

TLS is a cryptographic protocol that provides end-to-end security of data sent between applications over the Internet. It is mostly familiar to users through its use in secure web browsing.

19. ### What is a network protocol?

A network protocol is an established set of rules that determine how data is transmitted between different devices in the same network.

20. ### What does a CMS actually do?

A CMS, short for content management system, is a software application that allows users to build and manage a website without having to code it from scratch, or know how to code at all. With a CMS, you can create, manage, modify, and publish content in a user-friendly interface.

