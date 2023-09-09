# Code Editor

## code block

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus mi erat, sodales sed cursus at, condimentum at neque. Vivamus sollicitudin felis nec commodo semper. 

```
{
  "firstName": "John",
  "lastName": "Smith",
  "age": 25
}
```

## With a lang specified

```javascript
import Navbar from './navbar'
import Footer from './footer'
 
export default function Layout({ children }) {
  return (
    <>
      <Navbar />
      <main>{children}</main>
      <Footer />
    </>
  )
}
```