<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 4


<!-- Su documentación aquí -->

<center> <h1>Actividad: Creación componente de lista de elementos.
 </h1> </center> 

Crear un componente de React llamado List que renderice una lista de elementos. El componente debe aceptar una prop llamada items que debe ser un array de objetos. Cada objeto del array debe tener los siguientes campos:

- name: El nombre del elemento.
- color: El color del elemento.

## List.jsx

```jsx
import React from 'react'

export default function List(props) {
    return (
        <>
            <ul>
                {
                    props.items.map((item) => {
                        return <li style={{ color: item.color }}>
                            <h3>{item.name}</h3>
                            
                        </li>
                    })
                }
            </ul>

        </>
    )
}


```

## App.jsx


```jsx
import { useState } from 'react'
import List from './components/List'



function App() {
const items = [
  {
    name:"manzana",
    color:"red",

  },
  {
    name:"Pera",
    color:"green",
   
  },
  {
    name:"Mango",
    color:"Yellow",
    
  },
  {
    name:"Naranja",
    color:"orange",
    
  }
]

  return (
    <>
    <List items = {items}/>
     
    </>
  )
}

export default App


```

## Muestra del sitio

![Muestra del sitio](https://firebasestorage.googleapis.com/v0/b/webii-836ac.appspot.com/o/muestra%20lista.png?alt=media&token=4faf2dc1-1090-43ca-b8cb-9f23dc9085c0&_gl=1*12mqz4x*_ga*OTQ2NDQzMzQwLjE2OTYwODUyMTE.*_ga_CW55HF8NVT*MTY5ODQ1MjA2My41LjEuMTY5ODQ1MjA4OC4zNS4wLjA.)








