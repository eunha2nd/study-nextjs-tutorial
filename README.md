# Next.js Tutorial Summary
* [Learn](https://nextjs.org/learn/basics/getting-started)

## Getting Started
```
npm init -y
npm install --save react react-dom next
mkdir pages
```
* Handling Errors:
By default, Next.js will track errors like these and show it in the browser. This helps you identify errors and fix them quickly.

**Once you fix the issue, the page will appear instantly without a full page reload.**

## Navigate Between pages
* Client-Side History Support:
When you hit the Back button, it navigates the page to the index page entirely via the client; **next/link does all the location.history handling for you.**

You don't need to write even a single line of client-side routing code.

* Link is Just a Higher Order Component (HOC):
Actually, **the title prop on next/link component has no effect. That's because next/link is just a [higher order component](https://reactjs.org/docs/higher-order-components.html)** which only accepts the "href" and some similar props. In this case, the child of the next/link component is the anchor tag.

* Link Works With Anything:
Just like a button, **you can place any of your custom React components or even a  div within a Link.**
