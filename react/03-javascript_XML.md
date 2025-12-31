# JSX - JavaScript XML
-It lets you write HTML - like markup language inside Javascript file

## Rules of JSX
1. Return a single root element
   - To return multiple elements from a component, wrap them with a single parent tag.
   -  you can write <> and </> instead of `<div>`, it is known as **fragment**
2. Close all the tags
   - JSX requires tags to be explicitly closed
   - self-closing tags like `<img>` must become `<img />`, and wrapping tags like `<li>oranges` must be written as `<li>oranges</li>`
3. camelCase in most of the things
   - many HTML and SVG attributes are written in camelCase
   - For example, instead of `stroke-width` you use `strokeWidth`
   - since `class` is a reserved word, in React you write `className` instead

> Pro-tip: Use a JSX Converter 