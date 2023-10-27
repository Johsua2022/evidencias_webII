<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 3 


<!-- Su documentación aquí -->

### Actividad: Sitio Web de películas utilizando React Bootstrap.

Esta actividad se realiza para crear un sitio de peliculas utilizando React y Bootstrap
y a continuacion se ponen los componentes necesarios para que el sitio funcione.

## MovieCard.jsx

```jsx
(
import React from 'react'
import { Card } from "react-bootstrap";

export default function MovieCard({ title, description, imageUrl }) {
    return (
        <Card>
            <Card.Img variant="top" src={imageUrl} />
            <Card.Body>
                <Card.Title>{title}</Card.Title>
                <Card.Text>{description}</Card.Text>
            </Card.Body>
        </Card>
    )
}
)
```







