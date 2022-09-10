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
- [14 Difference between MVC and MVVM?](#difference-between-mvc-and-mvvm)
- [15 What is the advantage of functional programming?](#what-is-the-advantage-of-functional-programming)
- [16 Which is better XML or JSON?](#which-is-better-xml-or-json)
- [17 What is RESTful API?](#what-is-restful-api)
- [18 What is meant by test coverage?](#what-is-meant-by-test-coverage)
- [19 What is integration testing?](#what-is-integration-testing)
- [20 What does a templating engine do?](#what-does-a-templating-engine-do)
- [21 What means single-page application?](#what-means-single-page-application)
- [22 What is DNS used for?](#what-is-dns-used-for)
- [23 What does headless mean in software?](#what-does-headless-mean-in-software)
- [24 Why do CORS occur?](#why-do-cors-occur)
- [25 Who benefits from accessibility?](#who-benefits-from-accessibility)
- [26 What is a web browser API?](#what-is-a-web-browser-api)
- [27 What is a static site generator?](#what-is-a-static-site-generator)
- [28 What is a static website?](#what-is-a-static-website)
- [29 What are the pros and cons of using a static site generator?](#what-are-the-pros-and-cons-of-using-a-static-site-generator)
- [30 What is Jamstack used for?](#what-is-jamstack-used-for)
- [31 What is Markdown?](#what-is-markdown)
- [32 What is a CDN?](#what-is-a-cdn)
- [33 What are the benefits of using a CDN?](#what-are-the-benefits-of-using-a-cdn)
- [34 How do I use headless browser?](#how-do-i-use-headless-browser)
- [35 How does a CDN work?](#how-does-a-cdn-work)
- [36 What is difference between package json and package lock json?](#what-is-difference-between-package-json-and-package-lock-json)
- [37 Why Progressive Web Apps?](#why-progressive-web-apps)
- [38 How progressive web app works?](#how-progressive-web-app-works)
- [39 What is manifest JSON in web?](#what-is-manifest-json-in-web)
- [40 What is nodejs?](#what-is-nodejs)
- [41 What is nodejs used for?](#what-is-nodejs-used-for)
- [42 What DO module bundlers do?](#what-do-module-bundlers-do)
- [43 What is a package?](#what-is-a-package)
- [44 What is gulp used for?](#what-is-gulp-used-for)
- [45 What is WebView used for?](#what-is-webview-used-for)
- [46 What is the benefit of software testing?](#what-is-the-benefit-of-software-testing)
- [47 How does DNS work?](#how-does-dns-work)
- [48 What is serverless](#what-is-serverless)
- [49 What is edge computing?](#what-is-edge-computing)
- [50 What is SSL?](#what-is-ssl)
- [51 How does streaming work?](#how-does-streaming-work)
- [52 What is HTTP live streaming (HLS)?](#what-is-http-live-streaming-hls)
- [53 What is web vitals ?](#what-is-web-vitals)
- [54 What are the 3 Core Web Vitals?](#what-are-the-3-core-web-vitals)
- [55 What is the CSS box model?](#what-is-the-css-box-model)
- [56 What is the difference HTTP and https?](#what-is-the-difference-http-and-https)
- [57 What are the SEO best practices](#what-are-the-seo-best-practices)
- [58 How can increase code manage maintainability ?](#how-can-increase-code-manage-maintainability)
- [59 What is TLS (Transport Layer Security)?](#what-is-tls-transport-layer-security)
- [60 What is a network protocol?](#what-is-a-network-protocol)
- [61 What does a CMS actually do?](#what-does-a-cms-actually-do)
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

DOM (Document Object Model) is a Tree representation of the page, starting from the `<html>` tag, going down into every child, which are called nodes. It's kept in the browser memory, and directly linked to what you see in a page.

14. ### Difference between MVC and MVVM?

Difference between MVC and MVVM

| MVC                                                 | MVVM                                                 |
| --------------------------------------------------- | ---------------------------------------------------- |
| ViewModel encapsulates presentation login and state | The controller is responsible for the business logic |
| ViewModel is optional Pattern                       | Controller is a must                                 |
| User hits the view first                            | User hits the controller first                       |

15. ### What is the advantage of functional programming?

Functional programming (FP) is a type of paradigm or pattern in computer science. Everything is done with the help of functions in FP and the basic building blocks are functions only.

- It reduces complex problems into simple pieces.
- It helps us to debug the code quickly.
- It helps us to solve problems by breaking down the problem into smaller and smaller pieces effectively in simpler way.
- It improves modularity and reusability of the code.
- Some programming languages support nested functions which improve maintainability of the code.

**Example:**

```javascript
function add(a, b) {
	return a + b
}

function multiply(a, b) {
	return a * b
}

function subtract(a, b) {
	return a - b
}
```

16. ### Which is better XML or JSON?

_JSON is best for simple applications,_ developed to satisfy simple requirements surrounding data interchange. XML is best for applications with complex requirements surrounding data interchange, such as in enterprise.

Differences between JSON and XML:
| JSON | XML |
| ---- | ---- |
| JSON doesn't use end tags | XML uses end tags |
| JSON can use arrays syntax | Normally XML can't have arrays syntax |
| JSON parse is easier | XML parse is much more difficult |

**Example of JSON:**

```javascript
{
    "name": "John",
    "age": 30,
    "cars": [
        "Ford",
        "BMW",
        "Fiat"
    ]
}
```

**Example of XML:**

```xml
<person>
    <name>John</name>
    <age>30</age>
    <cars>
        <car>Ford</car>
        <car>BMW</car>
        <car>Fiat</car>
    </cars>
</person>
```

17. ### What is RESTful API?

A REST API is an application programming interface (API) that provides the ability to read and write data from a server that conforms to the constraints of REST architectural style and allows the client to interact with the server in a uniform way.

18. ### What is meant by test coverage?

Test coverage is defined as a technique which determines whether our test cases are actually covering the application code and how much code is exercised when we run those test cases. If there are 10 requirements and 100 tests created and if 90 tests are executed then test coverage is 90%

19. ### What is integration testing?

A testing team interacts with an app and its units via the user interface – by clicking on buttons and links, scrolling, swiping, etc. They don't need to know how code works or consider the backend part of the components. They can focus on the user interface and the interaction with the app to test the app and its functionality.

20. ### What does a templating engine do?

A template engine enables you to use static template files in your application. At runtime, the template engine replaces variables in a template file with actual values, and transforms the template into an HTML file sent to the client. This approach makes it easier to design an HTML page.

Most popular template engines are:

- [Mustache](https://mustache.github.io/)
- [Handlebars](https://handlebarsjs.com/)
- [Twig](https://twig.sensiolabs.org/)
- [Nunjucks](https://nunjucks.org/)
- [Jinja](https://jinja.pocoo.org/)
- [EJS](https://www.embeddedjs.com/)
- [Dust](https://dustjs.com/)
- [Liquid](https://www.liquidengine.com/)
- [JSP](https://www.jsp.org/)
- [pug](https://pugjs.org/)

21. ### What means single-page application?

A single-page application is an app that doesn't need to reload the page during its use and works within a browser. Think of the apps you use daily: Facebook, Maps, Gmail, Twitter, Google Drive, or even GitHub. All these are examples of a SPA

22. ### What is DNS used for?

DNS, or the Domain name system, translates a domain name into an IP address. for example, www.google.com is translated into an IP address of 0000.0000.0000.0001 this kind of IP address.

23. ### What does headless mean in software?

Headless software (e.g. "headless browser" or "headless Linux",) is software capable of working on a device without a graphical user interface. Such software receives inputs and provides output through other interfaces like network or serial port and is common on servers and embedded devices.

24. ### Why do CORS occur?

Browser has an same-origin policy rule that prohibits cross-origin requests. This is because the browser's security model which allows to request resources from same origin only. When a browser requests a resource from a different origin, it has to send a CORS request to the server.

25. ### Who benefits from accessibility?

The most obvious benefit of web accessibility is that it helps people with disabilities enjoy your website’s content, products, and services. However, the advantages of web accessibility aren’t limited to their immediate impact for people with disabilities — they also benefit Improving SEO, user experience, increasing usability, and more.

26. ### What is a web browser API?

Web API is provided by the browser to allow developers to interact with the browser and its features. For example, the [Geolocation API](https://developer.mozilla.org/en-US/docs/Web/API/Geolocation_API) allows you to access the user's location, and the [Canvas API](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API) allows you to draw graphics and animations.

27. ### What is a static site generator?

A static site generator is a tool that generates a full static HTML website based on raw data and a set of templates. Essentially, a static site generator automates the task of coding individual HTML pages and gets those pages ready to serve to users ahead of time. Because these HTML pages are pre-built, they can load very quickly in users' browsers.

28. ### What is a static website?

A static website is made up of one or more HTML webpages that load the same way every time. Static websites contrast with dynamic websites, which load differently based on any number of changing data inputs, such as the user's location, the time of day, or user actions. While static webpages are simple HTML files that can load quickly, dynamic webpages require the execution of JavaScript code within the browser in order to render.

29. ### What are the pros and cons of using a static site generator?

### **Pros**

- **Performance:** Because static site generators create webpages in advance instead of on demand (as with a CMS), webpages load slightly faster in users' browsers.

- **Customization:** Developers can create any template they want. They are not limited by the fields provided by a CMS, nor by a CMS's built-in templates.

- **Lighter backend:** Static websites are lightweight and do not require as much code to run on the server side, whereas CMS-based websites constantly query the server side for content.

### **Cons**

- **Few or no pre-built templates:** The downside of unlimited customization is that it can take longer to get started. Many static site generators do not come with templates, and developers will have to spend a lot of time building them from scratch at first.
-
- **No user-friendly interface:** It is harder for non-developer users to publish content using a static site generator. There is no CMS interface, and working with raw unformatted data may be intimidating for users. In addition, developer support is often necessary for making website updates.

30. ### What is Jamstack used for?

JAMstack is an approach to frontend web development (the construction of content and interfaces that users interact with). It allows developers to quickly create and efficiently serve static websites to users.

In a JAMstack web application, as much HTML as possible is pre-built and stored in a content delivery network (CDN). Instead of running a monolithic backend application on the server side to generate dynamic content, dynamic components of the application are based on APIs. Ideally, this results in a much faster user experience and a much simpler developer experience.

31. ### What is Markdown?

Markdown is a widely used, simple markup language for formatting text. Many developers today prefer using Markdown to traditional HTML when coding content, and many static site generators support Markdown.

32. ### What is a CDN?

A content delivery network (CDN) refers to a geographically distributed group of servers which work together to provide fast delivery of Internet content. A CDN allows for the quick transfer of assets needed for loading Internet content including HTML pages, javascript files, stylesheets, images, and videos.

33. ### What are the benefits of using a CDN?

- **Improving website load times**
  CDN can improve website load times by caching content and serving it from the closest server to the user. This reduces the time it takes to load a website and improves the user experience.
- **Reduce bandwidth costs**
  Through caching and other optimizations, CDNs are able to reduce the amount of data an origin server must provide, thus reducing hosting costs for website.
- **Improving website security**
  CDNs can provide additional security by blocking malicious traffic and preventing DDoS attacks.

34. ### How do I use headless browser?

Headless browsers are a web browser without a graphical user interface that can be controlled from a command line interface programmatically for the purpose of web page automation (e.g., functional testing, scraping, unit testing, etc.). Think of headless browsers as a browser that you can run programmatically from the command line that can retrieve and traverse web page code.

The most common headless browsers are:

- Headless Chromium
- Puppeteer

35. ### How does a CDN work?

At its core, a CDN is a network of servers linked together with the goal of delivering content as quickly, cheaply, reliably, and securely as possible. In order to improve speed and connectivity, a CDN will place servers at the exchange points between different networks.

A CDN is a network of servers that distributes content from an “origin” server throughout the world by caching content close to where each end user is accessing the internet via a web-enabled device. The content they request is first stored on the origin server and is then replicated and stored elsewhere as needed.

36. ### What is difference between package json and package lock json?

In NodejS we have two files package.json and package-lock.json. Both files are used to manage dependencies of a project. But there is a difference between them.

**Difference in Tabular Form**
| package.json | package-lock.json |
| :-------------------------------------------------------- | :------------------------------------------------------------- |
| It contains basic information about the project. | It describes the exact tree that was generated to allow subsequent installs to have the identical tree. |
| It is mandatory for every project. | It is automatically generated for those operations where npm modifies either node_modules tree or package.json. |
| It records important metadata about the project. | It allows future devs to install the same dependencies in the project.
| It contains information such as name, description, author, script, and dependencies. | It contains the name, dependencies, and locked version of the project.

37. ### Why Progressive Web Apps?

Progressive Apps allow users to install app without going to app store. User will be able getting app experience immediately. Progressive app are now supported by all major browsers.

38. ### How progressive web app works?

The progressive web app works with native web technologies. It works with service workers, and app manifest. Service workers are used to caching the app and making it available offline. App manifest is used to provide information about the app.

39. ### What is manifest JSON in web?

The web app manifest is a JSON file that tells the browser about your Progressive Web App and how it should behave when installed on the user's desktop or mobile device.

**Example**

```json
{
	"name": "Weather",
	"short_name": "Weather",
	"start_url": "/?source=pwa",
	"display": "standalone",
	"theme_color": "#2f3ba2",
	"background_color": "#2f3ba2"
}
```

Here we have a manifest file for a weather app. It has a name, a short name, a start URL, a display mode, a theme color, and a background color. now it's can getting appearance depending on the manifest file.

40. ### What is nodejs?

Node.js is an open-source, cross-platform, back-end, JavaScript runtime program that executes JavaScript codes outside of a web browser.

41. ### What is nodejs used for?

Node.js is most often used to easily build and scale network applications. Node.js creates models that are lightweight and efficient which are ideal for data-intensive and real-time applications.

42. ### What DO module bundlers do?

Module bundlers are the way to organize and combine many files of JavaScript code into one file. A JavaScript bundler can be used when your project becomes too large for a single file or when you're working with libraries that have multiple dependencies.

43. ### What is a package?

A package is a reusable piece of software which can be downloaded from a global registry into a developer’s local environment. Each package may or may not depend on other packages.

44. ### What is gulp used for?

Gulp is a tool that helps us out with several tasks when it comes to web development. It's often used to do front end tasks like: Spinning up a web server. Reloading the browser automatically whenever a file is saved.

45. ### What is WebView used for?

Webviews are used by a native OS, in a native application, to run web pages. Think of a webview like an iframe or a single tab from a web browser that is embedded in a native application running on a device (e.g., iOS, android, windows).

46. ### What is the benefit of software testing?

A properly tested software product ensures dependability, security, and high performance, which leads to time savings, cost effectiveness, and customer satisfaction. It happens to be an integral part of the process.

47. ### How does DNS work?

The process of DNS resolution is a bit like a phone book. When you want to call someone, you look up their number in the phone book. When you want to visit a website, you look up its IP address in the DNS.

DNS resolution involves converting a hostname (such as www.example.com) into a computer-friendly IP address (such as 192.168.1.1). An IP address is given to each device on the Internet, and that address is necessary to find the appropriate Internet device.

48. ### What is serverless

Server-less does not mean that there is no server. It means that the developer does not have to worry about the server. The server is managed by the cloud provider. The developer only needs to focus on the application logic.

Serverless is a cloud computing execution model in which the cloud provider dynamically manages the allocation and provisioning of servers. A serverless platform typically abstracts away the server and infrastructure management, and lets developers deploy code on demand. The serverless platform automatically scales the infrastructure up and down, and bills the developer based on the actual amount of resources consumed.

**Some of the benefits of serverless are:**

- No need to manage servers
- No need to worry about scaling
- No need to worry about security
- No need to worry about availability
- No need to worry about performance
- No need to worry about cost
- No need to worry about monitoring

49. ### What is edge computing?

Edge computing is a networking philosophy focused on bringing computing as close to the source of data as possible in order to reduce latency and bandwidth use

50. ### What is SSL?

SSL, or Secure Sockets Layer, is an encryption-based Internet security protocol. It is used to secure communications between a client and a server. SSL is used to protect sensitive information such as credit card numbers, social security numbers, and login credentials. It is also used to authenticate websites and ensure that the data being sent is not being intercepted by a third party.

51. ### How does streaming work?

Just like other data that's sent over the Internet, audio and video data is broken down into data packets. Each packet contains a small piece of the file, and an audio or video player in the browser on the client device takes the flow of data packets and interprets them as video or audio.

52. ### What is HTTP live streaming (HLS)?

HTTP live streaming (HLS) is one of the most widely used video streaming protocols. Although it is called HTTP "live" streaming, it is used for both on-demand streaming and live streaming. HLS breaks down video files into smaller downloadable HTTP files and delivers them using the HTTP protocol. Client devices load these HTTP files and then play them back as video.

53. ### What is web vitals ?

It's an way to measure and report the site performance. With this Help we can easily understand the performance of the site and can improve it. In browser we can see the performance of the site by using the developer tools.

54. ### What are the 3 Core Web Vitals?

To provide a good user experience. There are 3 stage we need to focus on. Loading, Interactivity and Visual Stability. In Core Web Vitals that are called as LCP, FID and CLS.

55. ### What is the CSS box model?

The CSS box model is essentially a box that wraps around every HTML element. It consists of: margins, borders, padding, and the actual content.

56. ### What is the difference HTTP and https?

HTTPS is HTTP with encryption and verification. The only difference between the two protocols is that HTTPS uses TLS (SSL) to encrypt normal HTTP requests and responses, and to digitally sign those requests and responses. As a result, HTTPS is far more secure than HTTP.

57. ### What are the SEO best practices

1. Use a descriptive title
2. Optimize meta description
3. Image optimization and page speed
4. Build internal and external links structure
5. Make URL search engine friendly

58. ### How can increase code manage maintainability ?

1. Use human readable and sensible names
2. Minimize nested and conditional logic
3. Decouple and isolate code
4. Remove unused code
5. Separate configuration from code

59. ### What is TLS (Transport Layer Security)?

TLS is a cryptographic protocol that provides end-to-end security of data sent between applications over the Internet. It is mostly familiar to users through its use in secure web browsing.

60. ### What is a network protocol?

A network protocol is an established set of rules that determine how data is transmitted between different devices in the same network.

61. ### What does a CMS actually do?

A CMS, short for content management system, is a software application that allows users to build and manage a website without having to code it from scratch, or know how to code at all. With a CMS, you can create, manage, modify, and publish content in a user-friendly interface.

