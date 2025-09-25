# Software Engineer Interview Q&A - Interactive Study Guide

> **📚 Study Mode**: Click on questions to reveal answers, track your progress, and test your knowledge!

---

## 📊 Progress Tracker

- **🟢 Beginner**: 0/24 completed
- **🟡 Intermediate**: 0/20 completed
- **🔴 Advanced**: 0/20 completed

---

## 🎮 Quick Navigation

<details>
<summary><strong> Jump to Section</strong></summary>

- [🟢 Beginner Level](#-beginner-level)
  - [React.js](#reactjs-1)
  - [Vue.js](#vuejs-1)
  - [JavaScript](#javascript-1)
  - [TypeScript](#typescript-1)
- [🟡 Intermediate Level](#-intermediate-level)
  - [React.js](#reactjs-2)
  - [Vue.js](#vuejs-2)
  - [JavaScript](#javascript-2)
  - [TypeScript](#typescript-2)
- [🔴 Advanced Level](#-advanced-level)
  - [React.js](#reactjs-3)
  - [Vue.js](#vuejs-3)
  - [JavaScript](#javascript-3)
  - [TypeScript](#typescript-3)

</details>

---

## 🟢 Beginner Level

### React.js

<details>
<summary><strong>❓ What problems does React solve?</strong></summary>

**Answer:** Declarative UI, component reuse, predictable state flow, efficient DOM updates.

**💡 Key Points:**

- Makes UI development more predictable
- Enables component-based architecture
- Handles complex state management
- Optimizes DOM updates automatically

**🔗 Related Topics:** Virtual DOM, Component Lifecycle, State Management

</details>

<details>
<summary><strong>❓ Difference between function and class components?</strong></summary>

**Answer:** Function components (with hooks) are simpler; class components are older, less preferred today.

**💡 Key Points:**

- Function components: Modern, hooks-based, simpler syntax
- Class components: Legacy, lifecycle methods, more verbose
- Hooks provide same functionality as lifecycle methods

**🔗 Related Topics:** Hooks, Lifecycle Methods, Modern React Patterns

</details>

<details>
<summary><strong>❓ What is JSX?</strong></summary>

**Answer:** Syntax extension for writing HTML-like code inside JavaScript.

**💡 Key Points:**

- Not HTML - it's JavaScript
- Must return single element or fragment
- Can embed JavaScript expressions with `{}`
- Gets transpiled to `React.createElement()` calls

**🔗 Related Topics:** Babel, Transpilation, React.createElement

</details>

<details>
<summary><strong>❓ What are props?</strong></summary>

**Answer:** Inputs passed to components for configuration.

** Key Points:**

- Read-only data passed down from parent
- Can be any JavaScript value
- Enable component reusability
- Follow unidirectional data flow

**🔗 Related Topics:** Component Communication, Data Flow, Immutability

</details>

<details>
<summary><strong>❓ What is state?</strong></summary>

**Answer:** Local, mutable data inside a component that triggers re-renders when changed.

** Key Points:**

- Component's internal data
- Triggers re-renders when updated
- Managed with `useState` hook
- Should be immutable updates

**🔗 Related Topics:** useState Hook, Re-rendering, Immutability

</details>

<details>
<summary><strong>❓ Controlled vs uncontrolled inputs?</strong></summary>

**Answer:** Controlled = React state is the source of truth. Uncontrolled = DOM manages input, accessed with refs.

**💡 Key Points:**

- **Controlled**: Value controlled by React state
- **Uncontrolled**: DOM manages the value
- Controlled preferred for form validation
- Uncontrolled better for performance with large forms

**🔗 Related Topics:** Forms, Refs, Performance Optimization

</details>

---

### Vue.js

<details>
<summary><strong>❓ What is Vue.js?</strong></summary>

**Answer:** A progressive JS framework for building UIs.

**💡 Key Points:**

- Progressive: can be adopted incrementally
- Template-based with reactive data binding
- Smaller learning curve than React/Angular
- Excellent documentation and developer experience

**🔗 Related Topics:** Progressive Framework, Reactive Data Binding, Vue Ecosystem

</details>

<details>
<summary><strong>❓ What is a Single File Component (SFC)?</strong></summary>

**Answer:** `.vue` files containing `<template>`, `<script>`, and `<style>`.

**💡 Key Points:**

- All component code in one file
- Clear separation of concerns
- Scoped styles by default
- Easy to understand and maintain

** Related Topics:** Component Architecture, Scoped Styles, Vue CLI

</details>

<details>
<summary><strong>❓ Difference between Options API and Composition API?</strong></summary>

**Answer:** Options API organizes code by option (data, methods). Composition API organizes by logic/features using `setup()`.

**💡 Key Points:**

- **Options API**: Traditional, organized by type (data, methods, computed)
- **Composition API**: Modern, organized by feature/logic
- Composition API better for complex components
- Both can be used together

**🔗 Related Topics:** Vue 3, Setup Function, Code Organization

</details>

<details>
<summary><strong>❓ What is `v-model` used for?</strong></summary>

**Answer:** Two-way data binding between form inputs and state.

**💡 Key Points:**

- Syntactic sugar for `:value` + `@input`
- Works with custom components
- Handles different input types automatically
- Essential for form handling

**🔗 Related Topics:** Two-way Binding, Form Handling, Custom Components

</details>

---

### JavaScript

<details>
<summary><strong>❓ Difference between `var`, `let`, and `const`?</strong></summary>

**Answer:** `var` = function-scoped, hoisted. `let` = block-scoped, reassignable. `const` = block-scoped, not reassignable.

**💡 Key Points:**

- **var**: Function-scoped, hoisted, can be redeclared
- **let**: Block-scoped, not hoisted, can be reassigned
- **const**: Block-scoped, not hoisted, cannot be reassigned
- Prefer `const` by default, `let` when reassignment needed

**🔗 Related Topics:** Hoisting, Scope, Temporal Dead Zone

</details>

<details>
<summary><strong>❓ What is a closure?</strong></summary>

**Answer:** A function that "remembers" variables from its defining scope.

**💡 Key Points:**

- Function has access to outer scope even after outer function returns
- Enables data privacy and function factories
- Common in JavaScript due to lexical scoping
- Foundation for many advanced patterns

**🔗 Related Topics:** Lexical Scoping, Function Factories, Data Privacy

</details>

<details>
<summary><strong>❓ Difference between `==` and `===`?</strong></summary>

**Answer:** `==` does type coercion. `===` checks strict equality.

**💡 Key Points:**

- **==**: Loose equality with type coercion
- **===**: Strict equality without coercion
- Always prefer `===` to avoid unexpected behavior
- Type coercion can lead to bugs

**🔗 Related Topics:** Type Coercion, Strict Equality, Best Practices

</details>

---

### TypeScript

<details>
<summary><strong>❓ What is TypeScript?</strong></summary>

**Answer:** A superset of JavaScript adding static typing.

** Key Points:**

- Adds type system to JavaScript
- Compiles to plain JavaScript
- Catches errors at compile time
- Improves developer experience and code quality

**🔗 Related Topics:** Static Typing, Compilation, Type Safety

</details>

<details>
<summary><strong>❓ What are types vs interfaces?</strong></summary>

**Answer:** Both define shapes. `interface` is extendable/mergeable. `type` handles unions, intersections, mapped types.

** Key Points:**

- **interface**: Extendable, mergeable, better for object shapes
- **type**: More flexible, handles unions/intersections, computed types
- Use interface for object shapes, type for everything else
- Both compile to same JavaScript

**🔗 Related Topics:** Type Definitions, Union Types, Intersection Types

</details>

<details>
<summary><strong>❓ What is `any` vs `unknown`?</strong></summary>

**Answer:** `any` = opt-out of type checking. `unknown` = must narrow before using.

**💡 Key Points:**

- **any**: Disables type checking completely
- **unknown**: Safe top type, requires type narrowing
- Prefer `unknown` over `any` for better type safety
- `unknown` forces you to check types before use

**🔗 Related Topics:** Type Narrowing, Type Safety, Top Types

</details>

---

## 🟡 Intermediate Level

### React.js

<details>
<summary><strong>❓ What is reconciliation in React?</strong></summary>

**Answer:** React's diffing algorithm to update the DOM efficiently using keys.

**💡 Key Points:**

- Virtual DOM comparison process
- Uses keys to identify elements
- Minimizes DOM operations
- Batches updates for performance

**🔗 Related Topics:** Virtual DOM, Diffing Algorithm, Performance

</details>

<details>
<summary><strong>❓ When to use `useMemo` vs `useCallback`?</strong></summary>

**Answer:** `useMemo` memoizes values. `useCallback` memoizes functions.

**💡 Key Points:**

- **useMemo**: Cache expensive calculations
- **useCallback**: Cache function references
- Both prevent unnecessary re-renders
- Use sparingly - optimization comes with cost

**🔗 Related Topics:** Memoization, Performance Optimization, Re-rendering

</details>

<details>
<summary><strong>❓ What's the difference between `useEffect` and `useLayoutEffect`?</strong></summary>

**Answer:** `useEffect` runs after paint (async). `useLayoutEffect` runs before paint (sync, blocking).

**💡 Key Points:**

- **useEffect**: Non-blocking, runs after DOM updates
- **useLayoutEffect**: Blocking, runs before browser paint
- Use `useLayoutEffect` for DOM measurements
- Most cases should use `useEffect`

**🔗 Related Topics:** Lifecycle Methods, DOM Manipulation, Performance

</details>

<details>
<summary><strong>❓ What is Context good for?</strong></summary>

**Answer:** App-wide state like theme or auth. Not good for frequent updates.

**💡 Key Points:**

- Avoids prop drilling
- Good for global state (theme, auth, language)
- Bad for frequently changing data
- Can cause unnecessary re-renders

**🔗 Related Topics:** State Management, Prop Drilling, Global State

</details>

<details>
<summary><strong>❓ What is list virtualization?</strong></summary>

**Answer:** Rendering only visible items for performance (e.g., `react-window`).

**💡 Key Points:**

- Only renders visible items in viewport
- Improves performance for large lists
- Libraries: react-window, react-virtualized
- Essential for thousands of items

**🔗 Related Topics:** Performance, Large Lists, Rendering Optimization

</details>

---

### Vue.js

<details>
<summary><strong>❓ What is `ref` vs `reactive`?</strong></summary>

**Answer:** `ref` wraps a primitive with `.value`. `reactive` makes an object deeply reactive.

**💡 Key Points:**

- **ref**: For primitives, accessed via `.value`
- **reactive**: For objects, direct property access
- `ref` can hold any value, `reactive` only objects
- Both create reactive references

**🔗 Related Topics:** Composition API, Reactivity, Primitive Values

</details>

<details>
<summary><strong>❓ What is a computed property?</strong></summary>

**Answer:** Cached derived state that updates when dependencies change.

**💡 Key Points:**

- Automatically cached based on dependencies
- Only recalculates when dependencies change
- More efficient than methods for derived data
- Available in both Options and Composition API

**🔗 Related Topics:** Caching, Derived State, Performance

</details>

<details>
<summary><strong>❓ What is Pinia?</strong></summary>

**Answer:** A modern state management library, replacement for Vuex.

**💡 Key Points:**

- Simpler than Vuex
- Better TypeScript support
- Composition API friendly
- Official recommendation for Vue 3

**🔗 Related Topics:** State Management, Vuex, Global State

</details>

<details>
<summary><strong>❓ Difference between `watch` and `watchEffect`?</strong></summary>

**Answer:** `watch` = observe explicit sources. `watchEffect` = tracks dependencies automatically.

**💡 Key Points:**

- **watch**: Explicit source, more control
- **watchEffect**: Automatic dependency tracking
- `watch` better for specific reactive sources
- `watchEffect` better for side effects

**🔗 Related Topics:** Side Effects, Dependency Tracking, Reactivity

</details>

---

### JavaScript

<details>
<summary><strong>❓ Explain the Event Loop.</strong></summary>

**Answer:** Manages call stack, Web APIs, and task queues (macro & microtasks).

**💡 Key Points:**

- Call Stack: Executes synchronous code
- Web APIs: Handle async operations
- Task Queues: Macro (setTimeout) and Micro (Promises)
- Microtasks have higher priority than macrotasks

**🔗 Related Topics:** Asynchronous JavaScript, Call Stack, Promises

</details>

<details>
<summary><strong>❓ Promise vs async/await?</strong></summary>

**Answer:** `async/await` is syntax sugar for promises, making code easier to read.

**💡 Key Points:**

- **Promises**: `.then()/.catch()` chains
- **async/await**: Syntactic sugar for promises
- `async/await` more readable for sequential async code
- Both handle asynchronous operations

**🔗 Related Topics:** Asynchronous Programming, Error Handling, Sequential Code

</details>

<details>
<summary><strong>❓ What is debouncing vs throttling?</strong></summary>

**Answer:** Debounce = run after inactivity. Throttle = limit executions per time window.

** Key Points:**

- **Debounce**: Wait for pause, then execute
- **Throttle**: Execute at most once per time period
- Debounce: search input, resize events
- Throttle: scroll events, API calls

**🔗 Related Topics:** Performance Optimization, Event Handling, Rate Limiting

</details>

<details>
<summary><strong>❓ Difference between shallow vs deep copy?</strong></summary>

**Answer:** Shallow copies references. Deep recursively copies values.

**💡 Key Points:**

- **Shallow**: Copies first level, nested objects shared
- **Deep**: Recursively copies all levels
- Shallow: `Object.assign()`, spread operator
- Deep: `JSON.parse(JSON.stringify())`, libraries

**🔗 Related Topics:** Object Cloning, References, Immutability

</details>

---

### TypeScript

<details>
<summary><strong>❓ What are generics?</strong></summary>

**Answer:** Reusable, type-safe code (e.g., `Array<T>`).

**💡 Key Points:**

- Type parameters that can be specified later
- Enables reusable, type-safe code
- Common in collections: `Array<T>`, `Promise<T>`
- Maintains type safety while being flexible

**🔗 Related Topics:** Type Parameters, Reusable Code, Type Safety

</details>

<details>
<summary><strong>❓ What is a discriminated union?</strong></summary>

**Answer:** Union with a common literal field (`kind`) for safe narrowing.

** Key Points:**

- Union type with common discriminant property
- Enables type-safe narrowing with switch statements
- Pattern for representing different states
- Prevents invalid state combinations

**🔗 Related Topics:** Union Types, Type Narrowing, State Management

</details>

<details>
<summary><strong>❓ What is `never` used for?</strong></summary>

**Answer:** Represents values that never occur (e.g., exhaustive switch cases).

**💡 Key Points:**

- Bottom type - no values can be assigned
- Used for exhaustive checking
- Indicates unreachable code
- Helps catch incomplete switch statements

**🔗 Related Topics:** Bottom Types, Exhaustive Checking, Type Safety

</details>

<details>
<summary><strong>❓ Utility types examples?</strong></summary>

**Answer:** `Partial`, `Pick`, `Omit`, `Record`, `Readonly`.

**💡 Key Points:**

- **Partial<T>**: Makes all properties optional
- **Pick<T, K>**: Select specific properties
- **Omit<T, K>**: Exclude specific properties
- **Record<K, V>**: Object with specific key/value types
- **Readonly<T>**: Makes all properties readonly

**🔗 Related Topics:** Type Manipulation, Built-in Types, Type Utilities

</details>

---

## 🔴 Advanced Level

### React.js

<details>
<summary><strong>❓ What is Suspense used for?</strong></summary>

**Answer:** Asynchronous data fetching and code splitting with fallbacks.

**💡 Key Points:**

- Declarative loading states
- Works with React.lazy for code splitting
- Can be used for data fetching (experimental)
- Provides better UX with loading states

** Related Topics:** Code Splitting, Loading States, Concurrent Features

</details>

<details>
<summary><strong>❓ What causes hydration mismatch?</strong></summary>

**Answer:** Server-rendered markup differs from client-rendered markup.

**💡 Key Points:**

- Server and client render different HTML
- Common causes: Date/time, random values, browser APIs
- Can cause React warnings and bugs
- Use `useEffect` for client-only code

**🔗 Related Topics:** SSR, Hydration, Server-side Rendering

</details>

<details>
<summary><strong>❓ How to optimize large React apps?</strong></summary>

**Answer:** Code splitting, lazy loading, memoization, context splitting, virtualization.

**💡 Key Points:**

- **Code splitting**: Load code on demand
- **Lazy loading**: Load components when needed
- **Memoization**: Prevent unnecessary re-renders
- **Context splitting**: Separate contexts by concern
- **Virtualization**: Render only visible items

**🔗 Related Topics:** Performance, Bundle Size, Optimization Techniques

</details>

<details>
<summary><strong>❓ What are compound components?</strong></summary>

**Answer:** Components designed to work together via context (like `<Select>` + `<Option>`).

**💡 Key Points:**

- Multiple components that work together
- Share state via context
- Flexible API for complex UI patterns
- Examples: Select/Option, Tabs/TabPanel

**🔗 Related Topics:** Component Composition, Context API, Design Patterns

</details>

<details>
<summary><strong>❓ How do you handle focus and accessibility in React apps?</strong></summary>

**Answer:** Focus management on modals, ARIA roles, keyboard navigation, proper semantics.

**💡 Key Points:**

- **Focus management**: Trap focus in modals
- **ARIA roles**: Screen reader support
- **Keyboard navigation**: Tab order, keyboard shortcuts
- **Semantics**: Proper HTML elements
- **Testing**: Automated accessibility testing

**🔗 Related Topics:** Accessibility, ARIA, Focus Management, Inclusive Design

</details>

---

### Vue.js

<details>
<summary><strong>❓ How does Vue's reactivity work under the hood?</strong></summary>

**Answer:** Proxies track reads/writes, dependency collection, and trigger reactivity updates.

**💡 Key Points:**

- **Vue 2**: Object.defineProperty for reactivity
- **Vue 3**: Proxy API for better performance
- Tracks property access and modifications
- Automatically updates dependent components

**🔗 Related Topics:** Proxy API, Dependency Tracking, Performance

</details>

<details>
<summary><strong>❓ What are composables?</strong></summary>

**Answer:** Reusable functions (`useX`) encapsulating state and effects in Composition API.

**💡 Key Points:**

- Reusable logic functions
- Start with `use` prefix
- Can contain reactive state and side effects
- Enable better code organization and reuse

**🔗 Related Topics:** Composition API, Code Reuse, Custom Hooks

</details>

<details>
<summary><strong>❓ Pitfalls of destructuring reactive state?</strong></summary>

**Answer:** Loses reactivity unless using `toRefs`.

**💡 Key Points:**

- Destructuring breaks reactivity
- Use `toRefs()` to maintain reactivity
- Or access properties directly
- Common mistake in Composition API

**🔗 Related Topics:** Reactivity, Destructuring, toRefs

</details>

<details>
<summary><strong>❓ How does Vue Router handle navigation guards?</strong></summary>

**Answer:** Global (`beforeEach`), per-route, and in-component guards.

**💡 Key Points:**

- **Global guards**: `beforeEach`, `afterEach`
- **Per-route guards**: `beforeEnter`
- **In-component guards**: `beforeRouteEnter`, `beforeRouteUpdate`
- Used for authentication, permissions, data loading

**🔗 Related Topics:** Navigation, Authentication, Route Protection

</details>

---

### JavaScript

<details>
<summary><strong>❓ Explain prototypal inheritance.</strong></summary>

**Answer:** Objects delegate property lookups to their prototype via the chain.

**💡 Key Points:**

- Objects inherit from other objects
- Property lookup follows prototype chain
- `__proto__` or `Object.getPrototypeOf()`
- Foundation of JavaScript's inheritance model

**🔗 Related Topics:** Inheritance, Prototype Chain, Object Creation

</details>

<details>
<summary><strong>❓ What is tree-shaking?</strong></summary>

**Answer:** Bundlers remove unused ESM exports for smaller bundles.

**💡 Key Points:**

- Dead code elimination at build time
- Works with ES modules
- Reduces bundle size significantly
- Requires static analysis of imports/exports

**🔗 Related Topics:** Bundle Optimization, ES Modules, Build Tools

</details>

<details>
<summary><strong>❓ How would you implement memoization in JS?</strong></summary>

**Answer:** Cache results of expensive functions keyed by inputs.

**💡 Key Points:**

- Store function results in cache
- Check cache before computation
- Key by function arguments
- Trade memory for computation time

**🔗 Related Topics:** Caching, Performance, Function Optimization

</details>

<details>
<summary><strong>❓ Difference between Web Workers and Service Workers?</strong></summary>

**Answer:** Web Worker = background JS thread. Service Worker = network proxy layer, supports offline & caching.

**💡 Key Points:**

- **Web Workers**: Background threads, CPU-intensive tasks
- **Service Workers**: Network proxy, offline support, caching
- Web Workers: parallel processing
- Service Workers: PWA features, push notifications

**🔗 Related Topics:** Background Processing, PWA, Offline Support

</details>

---

### TypeScript

<details>
<summary><strong>❓ Difference between structural and nominal typing?</strong></summary>

**Answer:** TS is structural: types are compatible if shapes match.

**💡 Key Points:**

- **Structural**: Types compatible if they have same shape
- **Nominal**: Types compatible only if explicitly declared
- TypeScript uses structural typing
- Enables flexible type relationships

** Related Topics:** Type Systems, Type Compatibility, Duck Typing

</details>

<details>
<summary><strong>❓ What are mapped types?</strong></summary>

**Answer:** Generate new types by iterating over keys:

```ts
type Readonly<T> = { [K in keyof T]: Readonly<T[K]> };
```

**💡 Key Points:**

- Transform existing types by iterating over keys
- Use `[K in keyof T]` syntax
- Enable powerful type transformations
- Foundation for many utility types

**🔗 Related Topics:** Type Transformation, Utility Types, Keyof Operator

</details>

<details>
<summary><strong>❓ What is type narrowing?</strong></summary>

**Answer:** Refining unions using typeof, instanceof, or custom predicates.

**💡 Key Points:**

- Narrow broad types to specific types
- Use type guards: `typeof`, `instanceof`, custom predicates
- Enables type-safe operations
- Essential for working with union types

**🔗 Related Topics:** Type Guards, Union Types, Type Safety

</details>

<details>
<summary><strong>❓ How do you enforce exhaustive checks?</strong></summary>

**Answer:** Use never in switch default branch.

**💡 Key Points:**

- Use `never` type in default case
- Catches incomplete switch statements
- Ensures all cases are handled
- Compile-time safety for exhaustive checks

**🔗 Related Topics:** Exhaustive Checking, Never Type, Type Safety

</details>

<details>
<summary><strong>❓ What's the purpose of tsconfig.json strict flags?</strong></summary>

**Answer:** Prevent implicit any, enforce null checks, ensure safer type checking.

** Key Points:**

- **strict**: Enables all strict type checking options
- **noImplicitAny**: Prevents implicit any types
- **strictNullChecks**: Prevents null/undefined errors
- **strictFunctionTypes**: Stricter function type checking
- **noImplicitReturns**: Ensures all code paths return

**🔗 Related Topics:** Type Safety, Configuration, Best Practices

</details>

---

## 🎯 Study Tips

<details>
<summary><strong> How to Use This Guide</strong></summary>

1. **📖 Read First**: Click on questions to reveal answers
2. **🧠 Practice**: Try to answer before revealing
3. ** Take Notes**: Write down key concepts
4. **🔄 Review**: Come back to difficult topics
5. **🎯 Focus**: Spend more time on your weak areas

</details>

<details>
<summary><strong>🎯 Interview Preparation Strategy</strong></summary>

1. **Start with Basics**: Master beginner concepts first
2. **Build Up**: Progress through intermediate to advanced
3. **Practice Coding**: Implement examples and demos
4. **Mock Interviews**: Practice explaining concepts out loud
5. **Stay Updated**: Follow latest trends and updates

</details>

---

## 🔗 Additional Resources

- **📚 Documentation**: [React](https://react.dev/) | [Vue](https://vuejs.org/) | [TypeScript](https://www.typescriptlang.org/)
- **🎥 Video Tutorials**: Check the README file for YouTube links
- **📖 GitHub Repos**: See README for curated question repositories

---

_Happy studying! 🚀 Remember: understanding concepts is more important than memorizing answers._
