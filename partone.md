# Software Engineer Interview Q&A

---

## 🟢 Beginner Level

### React.js

- **What problems does React solve?**  
  Declarative UI, component reuse, predictable state flow, efficient DOM updates.

- **Difference between function and class components?**  
  Function components (with hooks) are simpler; class components are older, less preferred today.

- **What is JSX?**  
  Syntax extension for writing HTML-like code inside JavaScript.

- **What are props?**  
  Inputs passed to components for configuration.

- **What is state?**  
  Local, mutable data inside a component that triggers re-renders when changed.

- **Controlled vs uncontrolled inputs?**  
  Controlled = React state is the source of truth.  
  Uncontrolled = DOM manages input, accessed with refs.

---

### Vue.js

- **What is Vue.js?**  
  A progressive JS framework for building UIs.

- **What is a Single File Component (SFC)?**  
  `.vue` files containing `<template>`, `<script>`, and `<style>`.

- **Difference between Options API and Composition API?**  
  Options API organizes code by option (data, methods).  
  Composition API organizes by logic/features using `setup()`.

- **What is `v-model` used for?**  
  Two-way data binding between form inputs and state.

---

### JavaScript

- **Difference between `var`, `let`, and `const`?**  
  `var` = function-scoped, hoisted.  
  `let` = block-scoped, reassignable.  
  `const` = block-scoped, not reassignable.

- **What is a closure?**  
  A function that “remembers” variables from its defining scope.

- **Difference between `==` and `===`?**  
  `==` does type coercion.  
  `===` checks strict equality.

---

### TypeScript

- **What is TypeScript?**  
  A superset of JavaScript adding static typing.

- **What are types vs interfaces?**  
  Both define shapes.  
  `interface` is extendable/mergeable.  
  `type` handles unions, intersections, mapped types.

- **What is `any` vs `unknown`?**  
  `any` = opt-out of type checking.  
  `unknown` = must narrow before using.

---

## 🟡 Intermediate Level

### React.js

- **What is reconciliation in React?**  
  React’s diffing algorithm to update the DOM efficiently using keys.

- **When to use `useMemo` vs `useCallback`?**  
  `useMemo` memoizes values.  
  `useCallback` memoizes functions.

- **What’s the difference between `useEffect` and `useLayoutEffect`?**  
  `useEffect` runs after paint (async).  
  `useLayoutEffect` runs before paint (sync, blocking).

- **What is Context good for?**  
  App-wide state like theme or auth. Not good for frequent updates.

- **What is list virtualization?**  
  Rendering only visible items for performance (e.g., `react-window`).

---

### Vue.js

- **What is `ref` vs `reactive`?**  
  `ref` wraps a primitive with `.value`.  
  `reactive` makes an object deeply reactive.

- **What is a computed property?**  
  Cached derived state that updates when dependencies change.

- **What is Pinia?**  
  A modern state management library, replacement for Vuex.

- **Difference between `watch` and `watchEffect`?**  
  `watch` = observe explicit sources.  
  `watchEffect` = tracks dependencies automatically.

---

### JavaScript

- **Explain the Event Loop.**  
  Manages call stack, Web APIs, and task queues (macro & microtasks).

- **Promise vs async/await?**  
  `async/await` is syntax sugar for promises, making code easier to read.

- **What is debouncing vs throttling?**  
  Debounce = run after inactivity.  
  Throttle = limit executions per time window.

- **Difference between shallow vs deep copy?**  
  Shallow copies references.  
  Deep recursively copies values.

---

### TypeScript

- **What are generics?**  
  Reusable, type-safe code (e.g., `Array<T>`).

- **What is a discriminated union?**  
  Union with a common literal field (`kind`) for safe narrowing.

- **What is `never` used for?**  
  Represents values that never occur (e.g., exhaustive switch cases).

- **Utility types examples?**  
  `Partial`, `Pick`, `Omit`, `Record`, `Readonly`.

---

## 🔴 Advanced Level

### React.js

- **What is Suspense used for?**  
  Asynchronous data fetching and code splitting with fallbacks.

- **What causes hydration mismatch?**  
  Server-rendered markup differs from client-rendered markup.

- **How to optimize large React apps?**  
  Code splitting, lazy loading, memoization, context splitting, virtualization.

- **What are compound components?**  
  Components designed to work together via context (like `<Select>` + `<Option>`).

- **How do you handle focus and accessibility in React apps?**  
  Focus management on modals, ARIA roles, keyboard navigation, proper semantics.

---

### Vue.js

- **How does Vue’s reactivity work under the hood?**  
  Proxies track reads/writes, dependency collection, and trigger reactivity updates.

- **What are composables?**  
  Reusable functions (`useX`) encapsulating state and effects in Composition API.

- **Pitfalls of destructuring reactive state?**  
  Loses reactivity unless using `toRefs`.

- **How does Vue Router handle navigation guards?**  
  Global (`beforeEach`), per-route, and in-component guards.

---

### JavaScript

- **Explain prototypal inheritance.**  
  Objects delegate property lookups to their prototype via the chain.

- **What is tree-shaking?**  
  Bundlers remove unused ESM exports for smaller bundles.

- **How would you implement memoization in JS?**  
  Cache results of expensive functions keyed by inputs.

- **Difference between Web Workers and Service Workers?**  
  Web Worker = background JS thread.  
  Service Worker = network proxy layer, supports offline & caching.

---

### TypeScript

- **Difference between structural and nominal typing?**  
  TS is structural: types are compatible if shapes match.

- **What are mapped types?**  
  Generate new types by iterating over keys:

```ts
type Readonly<T> = { [K in keyof T]: Readonly<T[K]> };
```

- **What is type narrowing?**

Refining unions using typeof, instanceof, or custom predicates.

- **How do you enforce exhaustive checks?**
  Use never in switch default branch.

- **What’s the purpose of tsconfig.json strict flags?**
  Prevent implicit any, enforce null checks, ensure safer type checking.
