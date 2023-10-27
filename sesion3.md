<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 3 


<!-- Su documentación aquí -->

### Actividad: Sitio Web de películas utilizando React Bootstrap.

Esta actividad se realiza para crear un sitio de peliculas utilizando React y Bootstrap
y a continuacion se ponen los componentes necesarios para que el sitio funcione.

## MovieCard.jsx

```jsx

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

```

## Movielist.jsx

```jsx
import React from "react";
import MovieCard from "./MovieCard";
import { Container, Row, Col } from "react-bootstrap";

const movies = [
  {
    title: "Blue Beetle",
    description: "Un nuevo heroe de dc nace el escarabajo azul",
    imageUrl: "https://media.filmelier.com/tit/VgBT3G/poster/blue-beetle_C1ST5TQ.jpeg",
  },
  {
    title: "Titanic",
    description: "La trajica historia del barco que se hundio",
    imageUrl: "https://media.filmelier.com/tit/qRfqzk/poster/titanic_J3UxSzQ.jpeg",
  },
  {
    title: "Thor",
    description: "Cuenta la historia del Dios del trueno y su fiel martillo ",
    imageUrl: "https://media.filmelier.com/images/filmes/cartaz/thor39776.jpeg",
  },
  {
    title: "Harry Potter y la piedra filosofal",
    description: "Cuenta los inicios del famoso mago harry potter el niño que vivio",
    imageUrl: "https://media.filmelier.com/tit/8465/poster/harry-potter-y-la-piedra-filosofal_lORikZU.jpeg",
  },
  {
    title: "Capitan America el primer vengador",
    description: "Cuenta la historia del primer vengador el super soldado, el capitan america",
    imageUrl: "https://media.filmelier.com/images/filmes/cartaz/captain-america-the-first-avenger86868.jpeg",
  },
  {
    title: "Avatar el camino del agua",
    description: "La continuacion de la fantastica historia y de un nuevo mundo en pandora",
    imageUrl: "https://media.filmelier.com/tit/NMm0lG/poster/avatar-el-camino-del-agua_S_v7wyQ.jpeg",
      },
  // ... Agrega más películas aquí
];

```







