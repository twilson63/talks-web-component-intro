title: Intro to Web Components
author:
name: Tom Wilson
twitter: twilson63
output: index.html
controls: true

---

## What are web-components?

--

Web Component is a standard way to build components in the browser.

--

Each framework has it own way to build components

--

What if you could build
framework agnostic components, that could work in any framework or without a framework?

--

Web Components are a collection of four specifications:

* custom elements
* shadow dom
* html templates
* html imports\*

> We will be talking about custom elements, shadow dom and html templates.

--

### Custom Elements

The custom elements spec is how you register a custom element for your web page.

```js
customElements.define('hello-world', HelloWorld)
```

--

### Shadow DOM

Sandboxes the composition of what makes up a particular component.

--

### html templates

```html
<template>
  <slot />
</template>
```

--

## Why think about web-components?

--

### Features - Sharing Components

* Ability to pass properties to the component via attributes
* Ability to send events to parent components as handlers.
* Ability to pass children components to a custom component
* Ability to style inside the component

--

### Demo

Lets create a web-component using Lit-HTML

```js
mkdir jrs-timezone
cd jrs-timezone
yarn init -y
yarn add @polymer/lit-element
touch index.js
touch test.html
```

--

### Resources

* https://github.com/material-components/material-components-web-components
* https://github.com/Polymer/lit-element
* https://stenciljs.com/
* https://github.com/twilson63/tnw-timezone
