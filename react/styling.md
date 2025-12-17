# Styling
We can style the components in three ways: 
- by styling all the components globally in the common index.css file
- by creating a css file for each component separately
- by styling them inside the component itself.

Inside the component we can implement styling by:-
- Inline CSS styling
- Internal or Embedded CSS styling

Let us style the Navbar Component globally in index.css file
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
Now let's perform inline style in img tag:-
```
<img src={profilePic} alt="Noimage" style={{"height":"400px","width":"310px"}}/>
```

## Insert image
Just like the static folder in django, React has **assests** folder to store the images, videos etc.
- create a folder 'images' and place the required image inside it, here place your profile picture 'MyPic.jpeg'
-In the the required component (here Hero component), import the image, MyPic.jpeg by `import profilePic from "./assets/images/MyPic.jpeg"`
- In the img tag, give src as profilePic ie, `<img src={profilePic} alt="Noimage" />`

