<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 3 


<!-- Su documentación aquí -->

<center> <h1> Actividad: Sitio Web de películas utilizando React Bootstrap.</h1> </center> 

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

const MovieList = () => {
  return (
    <Container>
      <Row>
        {movies.map((movie, index) => (
          <Col key={index} xs={12} md={4}>
            <MovieCard
              title={movie.title}
              description={movie.description}
              imageUrl={movie.imageUrl}
            />
          </Col>
        ))}
      </Row>
    </Container>
  );
};
export default MovieList;

```
## App.jsx

```jsx
import './App.css'
import MovieList from './components/MovieList'

function App() {
  return (
    <>
      <div>
        <header>
          <h1>Películas</h1>
        </header>
        <main>
          <MovieList />
        </main>
      </div>
    </>
  )
}
export default App

```


## Muestra del sitio



![Muestra del sitio](https://firebasestorage.googleapis.com/v0/b/webii-836ac.appspot.com/o/sitio%20de%20peliculas.png?alt=media&token=f47a0b6d-f2ad-46f6-92c2-2a90bb646e9e&_gl=1*1o2ady*_ga*OTQ2NDQzMzQwLjE2OTYwODUyMTE.*_ga_CW55HF8NVT*MTY5ODQ0NzM1NC40LjEuMTY5ODQ0OTgzOC41Ni4wLjA.)







