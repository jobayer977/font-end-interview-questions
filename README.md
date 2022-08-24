# Frequently Asked Front End Questions 
 ### Resources 
 

 ## Table of Contents

- [1 What does client-side mean?](#what-does-client-side-mean)
- [2 What is node.js](#what-is-nodejs)
- [3 Is cross browser testing necessary?](#is-cross-browser-testing-necessary)
- [4 Why do we use unit testing?](#why-do-we-use-unit-testing)
- [5 What does server side mean?](#what-does-server-side-mean)
- [6 What does headless mean in software?](#what-does-headless-mean-in-software)
- [7 How do I use headless browser?](#how-do-i-use-headless-browser)
- [8 What is WebView used for?](#what-is-webview-used-for)
- [9 What is the difference HTTP and https?](#what-is-the-difference-http-and-https)
- [10 What is TLS (Transport Layer Security)?](#what-is-tls-transport-layer-security)
- [11 What is a network protocol?](#what-is-a-network-protocol)
- [12 What does a CMS actually do?](#what-does-a-cms-actually-do)
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

5. ### What does server side mean?

`server side` means everything that happens on the server, instead of on the client. In the past, nearly all business logic ran on the server side, and this included rendering dynamic webpages, interacting with databases, identity authentication, and push notifications.

6. ### What does headless mean in software?

Headless software (e.g. "headless browser" or "headless Linux",) is software capable of working on a device without a graphical user interface. Such software receives inputs and provides output through other interfaces like network or serial port and is common on servers and embedded devices.

7. ### How do I use headless browser?

Headless browsers are a web browser without a graphical user interface that can be controlled from a command line interface programmatically for the purpose of web page automation (e.g., functional testing, scraping, unit testing, etc.). Think of headless browsers as a browser that you can run programmatically from the command line that can retrieve and traverse web page code.

The most common headless browsers are:

- Headless Chromium
- Puppeteer

8. ### What is WebView used for?

Webviews are used by a native OS, in a native application, to run web pages. Think of a webview like an iframe or a single tab from a web browser that is embedded in a native application running on a device (e.g., iOS, android, windows).

9. ### What is the difference HTTP and https?

HTTPS is HTTP with encryption and verification. The only difference between the two protocols is that HTTPS uses TLS (SSL) to encrypt normal HTTP requests and responses, and to digitally sign those requests and responses. As a result, HTTPS is far more secure than HTTP.

10. ### What is TLS (Transport Layer Security)?

TLS is a cryptographic protocol that provides end-to-end security of data sent between applications over the Internet. It is mostly familiar to users through its use in secure web browsing.

11. ### What is a network protocol?

A network protocol is an established set of rules that determine how data is transmitted between different devices in the same network.

12. ### What does a CMS actually do?

A CMS, short for content management system, is a software application that allows users to build and manage a website without having to code it from scratch, or know how to code at all. With a CMS, you can create, manage, modify, and publish content in a user-friendly interface.

