# 401 Class-37: React 1
[Back to 401 Index](401-index.md)<br>


# ES6 Overview
## [ES6 Syntax and Feature Overview](https://www.taniarascia.com/es6-syntax-and-feature-overview/)

Really useful overview of writing ES6 and the key differences from ES5.



<br>
<br>

# React
## [React - Overview](https://reactjs.org/)
## [React - Hello World](https://reactjs.org/docs/hello-world.html)
Example of displaying "Hello, world!" to a page.
```
ReactDOM.render(
  <h1>Hello, world!</h1>,
  document.getElementById('root')
);

```
## [React - JSX](https://reactjs.org/docs/introducing-jsx.html)
Neither string nor HTML but is JSX.
```
const element = <h1>Hello, world!</h1>;
```
***JSX*** is a syntax extension to JavaScript. It's recommended to be used with React to describe what the UI should look like. It looks like a template language but comes with the power of JS.
<br>

React doesn’t require using JSX, but most people find it helpful as a visual aid when working with UI inside the JavaScript code. It also allows React to show more useful error and warning messages.
<br>

[Video Link: Pete Hunt: React: Rethinking best practices -- JSConf EU (Oct 30, 2013)](https://www.youtube.com/watch?v=x7cQ3mrcKaY&ab_channel=JSConf)
```
1. Build components not templates.
- Separation of concerns: Reduce coupling, increase cohesion.
-- Coupling:"The degree to which each program module relies on each of the other modules." ie. if you get a bug how many places do you need to go to fix it.
-- Cohesion: "The degree to which elements of a module belong together." ie. grouping related things in a module.
- Templates encourage a poor separation of concerns. (So are Angular-style directives.)
-- "View Model" tightly couples template to display logic.
-- Display logic and markup are inevitably tightly coupled.
-- Display logic and markup are highly cohesive. (They both show the UI)
- Templates separate technologies, not concerns. (And they do it by being deliberately underpowered.)
- Symptoms that your front-end technology is underpowered: Reliance on primitive abstractions (like{{>}}and{{#each}}) and Inventing lots of new concepts.
- The framework cannot know how to separate your concerns for you. ( It should only provide powerful, expressive tools fro the user to do it correctly.)
- This tool is a React component. (A highly cohesive building block for UIs loosely coupled with other components.)

- USE components to separate your concerns. (With the full power of JavaScript, not crippled templating language.)

- Components are composable. (They are, after all, units.)
- Keep you components small. (Only pul display logic in your components.)

- React.Dom is a way to access the DOM

- JSX is an optimal preprocessor to let you use HTML-like syntax.

- With JSX, it's easy for designers to contribute code.

- React is The accessibility of templates and the power of JavaScript

2. Re-render the whole app on every update 
- Building UIs is hard because there is so much state.
- Data changing over time is the root of all evil.
- When the data, changes, React re-renders the entire component.
-- That is, React components are basically just idempotent functions. (They describe you UI at any point in time, just ike a server-rendered app.)
- Re-rendering on every change makes things simpler. (No magical data binding. No dirty checking the model. No more explicit DOM operations - everything is declarative.)

3. Virtual DOM (Makes re-rendering on every change fast. (Makes re-rendering on every change fast.)
- Built a virtual DOM (and events system). (Optimized for performance and memory footprint.)
----- On every update... -----
-- React builds a new virtual DOM subtree
-- ... diffs it with the old one
-- ... computes the minimal set of DOM mutations and puts them in a queue.
-- ... and batch executes all updates
** React looks like the DOOM 3 engine haha ** 

- IT's FAST (Computes minimal DOM operations. 
    Batched reass and writes for optimal DOM performance. 
    Usually faster than manual DOM operations. 
    Automatic top-level event delegation(with cross-browser HTML5 events).
    Provides hooks for custom update logic(though they're almost never used).)

- The virtual DOM lets us do fun things. (It can run in Node.js. Optimizations based on app structure. Testability for free. SVG VML and <canvas> support.)
 KEY TAKEAWAYS

 Components, not templates.
 Re-render, don't mutate.
 Virtual DOM is simple and fast.
```

## [React - Rendering Elements](https://reactjs.org/docs/rendering-elements.html)
## [React - Components & Props](https://reactjs.org/docs/components-and-props.html)
## [React - State & Lifecycle](https://reactjs.org/docs/state-and-lifecycle.html)
## [React - Handling Events](https://reactjs.org/docs/handling-events.html)



<br>
<br>

# Tailwind CSS
## [Utility First CSS](https://tailwindcss.com/docs/utility-first)

## [Tailwind in a 15 minute video!](https://www.youtube.com/watch?v=6zIuAyLZPH0&ab_channel=BetterDev)

A different style of CSS Framework, a utility-first CSS framework for rapidly building custom designs. 

[My Tailwind Practice on CodePen](https://codepen.io/amberfalbo/pen/NWdaojP?editors=1100)

also download Tailwind
npm/poetry/pip install/add tailwindcss
- control bundle sizes





<br>
<br>

# Next.js
## [Learn Next.js](https://nextjs.org/learn/basics/create-nextjs-app)
## [Why to use Next.js -  10 min video!](https://www.youtube.com/watch?v=rtgbaKBhdkk&ab_channel=LeeRobinson)


<br>
<br>
<br>

[Back to 401 Index](401-index.md)