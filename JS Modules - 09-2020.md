What are modules? Modules are just JavaScript files with special import / export directives
Why modules?
Before modules: everything is global, scary
After modules: isolated, safe

Shout out MDN:
ADD TO CHAT: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Modules

.mjs vs .js

Talk about Babel, Webpack, commonjs, amd, etc.
Things got complicated

# DEMO (1)

- Create an `index.html` and `main.js` file with a `greet` function.
- Show how you can just drop the html file into the browser and JS script works.
- Now, add `type="module"` and remove `src=""` and show how you need a server because of CORS (review errors in console)
  CORS basically controls which domains can request your website resources (a security measure)
- Talk about serve (https://www.npmjs.com/package/serve)

## EXPORTING MODULE FEATURES:

- can use `var`, `let`,`const`, or `function`
- must be top-level (can't use export inside a function)
- can use single export statement at end of file:

```tsx
export { name, draw, reportArea, reportPerimeter };
```

From MDN:

- Exporting module features
- Importing features into your script
- - Note: In some module systems, you can omit the file extension and the dot (e.g. '/modules/square'). This doesn't work in native JavaScript modules.
- Applying the module to your HTML
- Other differences between modules and standard scripts
- Default exports versus named exports
  Avoiding naming conflicts
- Renaming imports and exports
- Creating a module object
- Modules and classes
- Aggregating modules
- Dynamic module loading
- Troubleshooting
- See also

## PART 2: What the community is doing

Skypack (formerly Pika)
https://www.skypack.dev/

Vite
https://github.com/vitejs/vite

SnowPack
https://www.snowpack.dev/
