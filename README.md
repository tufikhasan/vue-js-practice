# Vue js project install using - Vue 3 + Vite

- **Create:** `yarn create vite` OR `npm create vite`
- **Open project:** `cd project-name`
- **Install node modules:** `yarn install` OR `npm install`
- **Run project:** `yarn dev` OR `npm run dev`

## In Vue.js, the Options API and Composition API are two ways to structure and organize code in your components.

### 1. Options API:

The Options API is the traditional and original way of defining components in Vue.js. It involves using various options inside a component object, such as data, methods, computed, watch, etc.

**Pros:**
Familiar and easy for beginners.
Clear separation of concerns.

**Cons:**
Can become verbose and harder to maintain in large projects.
Logic related to a single concern may be spread across multiple options.

### 2. Composition API:

The Composition API was introduced in Vue 3 to provide a more flexible and scalable way to organize code in components. It allows you to logically group code by concern, making it easier to manage.

**Pros:**
More flexibility and better organization.
Logic is grouped by concern, promoting code readability.
Improved reusability of logic through composition functions.

**Cons:**
Learning curve for developers familiar with the Options API.

### Conclusion:

Choosing between the Options API and Composition API depends on the project's size, complexity, and the development team's familiarity. For small projects or when starting with Vue.js, the Options API might be sufficient. However, for larger projects, the Composition API provides a more scalable and maintainable approach. It's also worth noting that you can use both APIs in the same project if needed.
