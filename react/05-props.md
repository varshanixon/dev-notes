# Props 
- arguments passed into react components via HTML attributes
- props stands for properties
- used to pass data from parent component to child component

**Step 1:** In *App.jsx*, type the following inside the function App (above return()):
`const skillSets=["java","python","django","DRF","REAT","AWS","DOCKER"]`

**Step 2:** Convert `<Skills></Skills>` to `<Skills skillSets={skillSets}></Skills>`. Now {skillSets} is the prop,that is react sends one object to Skills.jsx, {skillSets: ["java", "python", "django", "DRF", "REAT", "AWS", "DOCKER"]}

**Step 3:** In *Skills.jsx*,
```
import React from 'react'

function Skills(props) {
  return (
    <div>
        <h1>SKills</h1>
        <h3>props.skillSets<h3>
    </div>
  )
}

export default Skills
```

## Destructuring
To unpack values from an array or properties from objects into distinct variables.
For example,

```
const fruits = ["Bananas", "Oranges", "Apples", "Mangos"];

// Destructuring
let [fruit1, fruit2] = fruits;

document.getElementById("demo").innerHTML = fruit1 + " " + fruit2;
```
**Result:**
Bananas Orange


In Skills.jsx, we can perform destructuring to make the code shorter and cleaner.

**Without Destructuring :**
```
function Skills(props) {
  console.log(props.skillSets);
}
```
**With Destructuring**
```
function Skills({skillSets}) {
  console.log(skillSets);
}
```
Here, it pulls skillSets out of props.
```
import React from 'react'

function Skills({skillSets}) { //Destructuring
  return (
    <div>
        <h1>Skills</h1>
        <h3>{skillSets.map(s=><span>{s} |</span>)}</h3>
    </div>
  )
}

export default Skills
```