# NuxtLayer

So far just an experimental Repository around NuxtLayers. The goal is to store them in their own directory and load them from there. The concept is great, we'll see how it goes.

🔗 [nuxt.com/docs/getting-started/layers](https://nuxt.com/docs/getting-started/layers)

```bash
# nuxt.config.js
export default defineNuxtConfig({
  extends: [
    'gh:AndiKod/NuxtLayer/hello', // Extend from a git repository sub-directory
  ]
})
```
Or, if you keep all your coding projects in the same folder, you can clone the repo at the same level, and import it from there. In that case, you will have to update manually from time to time, to get the new version.

```bash
# nuxt.config.js
export default defineNuxtConfig({
  extends: [
    '../NuxtLayer/hello', // Extend from a locally cloned repository sub-directory
  ]
})
```
Then, from the project that extends AndiKod/NuxtLayer, we can simply use whatever componenets or functionality we want. 

```bash
# Somewhere in a template.
<template>
  <HelloWorld />
</template>
```


