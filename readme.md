## What is Vue?

Vue is a frontend Javascript framework for building websites & user interfaces

* Vue is generally used to create single-page apps that run on the client, but can be used to create full stack applications by making HTTP requests to a backend server. Vue is popular with Node.js & Express (MEVN Stack)

* Vue can also run on the server-side by using a SSR framework like Nuxt

## Why Use Vue?
* Create dynamic frontend apps & websites
* Easy learning curve
* Easy to integrate with other projects
* Fast & lightweight
* Virtual DOM
* Extremely popular (and rising)
* Great community

## What should you know first?
Like with any framework, you should be comfortable with the underlying language first. In this case, that is JavaScript
* Javascript Fundamentals
* Async Programming (promises)
* Array Methods (forEach, map, filter, etc)
* Fetch API / HTTP Requests
* NPM (Node Package Manager)

## Basic Layout of a Vue Component

```(vuejs)
<template>
    <header>
        <h1>{{title}}</h1>
    </header>
</template>

<script>
export default {
    props: {
        title: String,
    }
}
</script>

<style scoped>
    header {
        display: flex;
        justify-content: space-between;
        align-items: center;
        margin-bottom: 20px;
    }
</style>

``` 
<br>

Components include a template for markup, logic including any state/data/methods as well as the styling for that component <br>

You can also pass "props" into a component <br>
```(vuejs)
<Header title="Task Tracker">
```

## Working With State / Data
Components can have their own state which can determine how a specific componentn behaves and what data is displayed <br>

Some state may be local to a specific component and some may be **"Global"** or **"app"** level state that needs to be shared with multiple components <br>

Vuex is a state manager for global state in larger applications

## Options API vs. Composition API
Vue 3 has the composition API, which aims to address code reusability and readability in Vue 3, especially in larger applications <br>

I will be creating a separate video to demonstrate the composition API. We will be using the tradisional options API for now hehehe.

## Vue CLI
Standard tooling for Vue.js development <br>
* Command line interface for creating Vue apps
* Dev server and easy production build 
* Optional GUI for managing Vue projects
* Integrated testing, TypeScript support, ESLint & more 

<br>

`
npm install -g @vue/cli <br>
// OR <br>
yarn global add @vue/cli <br>

vue create my-project
// OR <br>
vue ui
`