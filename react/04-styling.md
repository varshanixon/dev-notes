# Styling
We can style the components in three ways: 
- by styling all the components globally in the common index.css file
- by creating a css file for each component separately
- by styling them inside the component itself.

Inside the component we can implement styling by:-
- Inline CSS styling
- Internal or Embedded CSS styling

## Global Styling
Let us style the Navbar Component **globally** in index.css file
```
import React from 'react'

function Navbar() {
  return (
    <div className='nav'>
        <a href="">Home</a>
        <a href="">About</a>
        <a href="">Education</a>
        <a href="">Projects</a>
        <a href="">Skills</a>
    </div>
  )
}

export default Navbar
```

In index.css file,
```
.nav{
  display: flex;
  justify-content: space-between;
  border: 2px solid black;
  padding: 10px;
}
```

## Inline styling
Now let's perform **inline styling** in img tag:-
```
<img src={profilePic} alt="Noimage" style={{"height":"400px","width":"310px"}}/>
```

## Internal styling
```
import React from 'react'

function Project() {
  const headingStyle = {
    "textAlign":"center",
    "color":"purple",
    "textDecoration":"underline"
  }
  return (
    <div>
        <h1 style={headingStyle}>Projects</h1>
    </div>
  )
}

export default Project
```

## Module Styling
Another way of styling the component is through module 

```
import React from 'react'

function Project() {
  const headingStyle = {
    "textAlign":"center",
    "color":"purple",
    "textDecoration":"underline"
  }
  return (
    <div>
        <h1 style={headingStyle}>Projects</h1>
        <div className='card'>
            <h2 className='card-title'>ExpenseTracker</h2>
            <div className='card-body'>
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Quasi perferendis vitae suscipit, laudantium culpa, beatae tenetur quisquam labore 
                in minus amet odit ullam sint repellat dicta recusandae aperiam cumque autem!

            </div>

            <div className='card-footer'>
                <span>Python|</span>  <span>Django |</span> <span>HTMl |</span>
            </div>
        </div>
    </div>
  )
}

export default Project
```


To style the class card, create a project.module.css file
```
.card{
    border: 1px solid black;
    border-radius: 10px;
}
```

In Project.jsx file import the module. `import myStyle from './project.module.css'`

Now edit the className as myStyle.card. 
```
<div className={myStyle.card}>
  <h2 className='card-title'>ExpenseTracker</h2>
  <div className='card-body'>
    Lorem ipsum dolor sit amet consectetur adipisicing elit. Quasi perferendis vitae suscipit, laudantium culpa, beatae tenetur quisquam labore 
    in minus amet odit ullam sint repellat dicta recusandae aperiam cumque autem!
    </div>
    <div className='card-footer'>
        <span>Python|</span>  <span>Django |</span> <span>HTMl |</span>
    </div>
</div>
```



## Insert image
Just like the static folder in django, React has **assests** folder to store the images, videos etc.
- create a folder 'images' and place the required image inside it, here place your profile picture 'MyPic.jpeg'
-In the the required component (here Hero component), import the image, MyPic.jpeg by `import profilePic from "./assets/images/MyPic.jpeg"`
- In the img tag, give src as profilePic ie, `<img src={profilePic} alt="Noimage" />`

