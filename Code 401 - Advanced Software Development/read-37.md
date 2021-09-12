# About React

- Why JSX?
- Instead of artificially separating technologies by putting markup and logic in separate files, React separates concerns with loosely coupled units called “components” that contain both. We will come back to components in a further section, but if you’re not yet comfortable putting markup in JS, this talk might convince you otherwise.

Embedding Expressions in JSX
In the example below, we declare a variable called name and then use it inside JSX by wrapping it in curly braces:

```
` const name = 'Josh Perez'; const element =
Hello, {name}
;
ReactDOM.render( element, document.getElementById('root') );
```

![](https://fiverr-res.cloudinary.com/images/q_auto,f_auto/gigs/144940123/original/fec77fb06f00a67584ed21d339e0e0abbab4f7ab/build-fix-web-apps-and-websites-with-js-react-and-python.jpg)

` You can put any valid JavaScript expression inside the curly braces in JSX. For example, 2 + 2, user.firstName, or formatName(user) are all valid JavaScript expressions.

## JSX is an Expression Too

After compilation, JSX expressions become regular JavaScript function calls and evaluate to JavaScript objects.

## Specifying Attributes with JSX

You may use quotes to specify string literals as attributes:

const element = <div tabIndex="0"></div>;

## State and Lifecycle

Components let you split the UI into independent, reusable pieces, and think about each piece in isolation. This page provides an introduction to the idea of components. You can find a detailed component API reference here.

## Function and Class Components

The simplest way to define a component is to write a JavaScript function:

```
function Welcome(props) { return <h1>Hello, {props.name}</h1>; }
```

## Composing Components

Components can refer to other components in their output. This lets us use the same component abstraction for any level of detail. A button, a form, a dialog, a screen: in React apps, all those are commonly expressed as components.
