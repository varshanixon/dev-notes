# Project PortfolioSelf

- create React project 'PortfolioSelf'. Refer [getting_started](getting_started.md)
- create Navbar component (Navbar.jsx) and render it inside App Component.
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
- create another component Hero.jsx and render it inside App.jsx
```
import React from 'react'

function Hero() {
    const profileName = "Varsha Nixon"
    const profileTitle = ["Full Stack Python Developer", "Django & DRF","REST APIs","MySQL"]
  return (
    <div className='hero'>
        <div>
            <h2>Hi, I am {profileName}.</h2>
            {profileTitle.map(t=><span>{t}| </span>)}
        </div>
        <div className='hero-image'>
            <img src="" alt="Noimage" />
        </div>
    </div>
  )
}

export default Hero
```
