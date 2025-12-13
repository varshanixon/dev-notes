# React Introduction
- free and open source, front-end **JavaScript Library**
- to build single page applications
- uses reusable components
- creates a **Virtual DOM** in memory where all the manipulations are done, before making changes in the browser DOM.

## Components
- independent, reusable bits of code
- returns HTML
- 2 types:
  - Class Components
  - Function Components 
- Function components are preferred nowadays because they are clean & simple and does not require the use of **'this'** keyword.

### Creating Function Component (Navbar Component)
- Create a file Navbar.jsx (extension should be .jsx).
> **Note:** The component name should match the filename.
- Inside the file, type:-
  ```
  function Navbar(){
    return(
        <>
        Navbar Componenet
        <>This is Navbar...</>
        </>
    )
  }
  ```
