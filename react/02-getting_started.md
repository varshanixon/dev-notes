# Project Creation and 
- Step 1: Install node.js
> Node.js is a JS runtime environment designed to run JS outside web browser
- Step 2: Open cmd and go to the directory you want to create the project and perform the following:-
  - Enter `npm create vite@latest`command
  - Enter the project name, here 'PortfolioSelf'
  - Enter the package name, here 'portfolioself' (default)
  - Select the framework as 'React'
  - Select the variant as 'JavaScript'
  - Now change directory to project folder, here 'PortfolioSelf'
  - Enter the command `npm install` to install all the dependencies required
  - Enter `code .` to open the project in VS Code
- Step 3: Install ES7+React/Redux/React- Native Snippets
- Step 4: Open **App.jsx** file in **src** folder and clear all.
- Step 5: Create function App by typing `rfce`
- Step 6: Create a file **Navbar.jsx** in src folder and type rfce to create the **function Navbar**.
- Step 7: Import Navbar in App.jsx
```
import React from 'react'
import Navbar from './Navbar'

function App() {
  return (
    <div>
      <Navbar></Navbar>
    </div>
  )
}

export default App
```
- Step 8: Run `npm run dev` in the cmd terminal of VS Code

