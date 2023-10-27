<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 1 


<!-- Su documentación aquí -->
## 1.	¿Cuáles son los lenguajes de programación más comunes utilizados para el desarrollo web?
R/ los lenguajes de programación mas comunes para el desarrollo web son:
Html que es la base de toda la estructura de una pagina web, el CSS aunque no es un lenguaje como tal es el que se usa para dar estilo en las paginas web dando el formato al html. Y javascript es un lenguaje muy importante para el desarrollo web, también hay otros lenguajes como php ,java y c#.

## 2.	¿Qué es HTML y para qué se utiliza?
R/
HTML es la base para la programación web, se utiliza para dar estructura a las paginas dando un orden  y que se pueda mostrar el contenido correctamente en un navegador.
Se utiliza para estructurar el contenido, crear enlaces, insertar medios como imágenes y videos, formularios y entradas de usuarios.

## 3.	¿Qué es CSS y para qué se utiliza?
R/  CSS  no es un lenguaje como tal , pero se usa para dar estilo y un formato diferente al HTML. como centrado, estilos.

## 4.	¿Qué es JavaScript y para qué se utiliza?
R/ JavaScript es un lenguaje de programación muy utilizado para la web si no el mas importante para el desarrollo web, se utiliza para crear interacciones dinámicas, validación de formularios, animaciones y manipulación del DOM.

## 5.	¿Qué es un elemento HTML y cómo se crea?
R/ un elemento es una parte básica que tiene un significado y una función especifica están compuestos por etiquetas, contenido  y atributos.
Las etiquetas definen el tipo de elemento y rodean el contenido. Los atributos proporcionan información adicional sobre el elemento.
Un ejemplo de etiqueta es <p> que es la apertura y si dentro de esta etiqueta ponemos un texto este seria el contenido del elemento </p> y este seria el cierre de la etiqueta.

Un ejemplo de atributos es :  img src="imagen.jpg" alt="Descripción de la imagen", src y alt son atributos, y "imagen.jpg" y "Descripción de la imagen" son sus respectivos valores.

## 6.	¿Qué es una hoja de estilos CSS y cómo se enlaza a una página HTML?
R/ una hoja de estilos CSS es un archivo que contiene reglas de estilos que controlan el diseño de la pagina web modificando el HTML ,y dándole estilos de fuente, color , posicionamiento  y asi darle una mejor apariencia a nuestra pagina web.
Primero que crear un archivo con extensión .css, , ejemplo estilo.css y para enlazar en el archivo HTML creamos un elemento <link>para establecer una relación entre el archivo HTML y el CSS y un atributo ‘href’ que apunte a la ubicación del archivo .css y el atributo ‘rel’ debe ser “stylesheet.

## 7.	¿Qué son las funciones en JavaScript y cómo se crean?
R/ en JavaScript las funciones son bloques de código reutilizable que realizan tareas especificas, son parte importante de la programación con JavaScript
Se crean utilizando la palabra clave ‘ function’ seguido del nombre de la función
Una lista de paréntesis con los argumentos si los hay y un bloque de código cerrado entre llaves {}.

## 8.	¿Qué es una estructura de control de flujo en JavaScript y cómo se utiliza en una página web?

R/ Una estructura de control de flujo en JavaScript es un conjunto de instrucciones que permite controlar el orden en que se ejecutan las diferentes partes de un programa, y dependiendo de ciertas condiciones estas estructuras pueden tomar decisiones.
Existen estructuras condicionales, que permiten ejecutar diferentes bloques de códigos dependiendo de una condición si se cumple o no.
Los bucles que permiten repetir un bloque de código varias veces mientras se cumple una condición .
Y los switch que permite seleccionar un bloque de código para ejecutar basado en el valor de una expresión.


## 9.	¿Qué es una variable en JavaScript y cómo se declara?
R/ en JavaScript una variable es un contenedor donde se puede puede almacenar un dato pueden ser numero, cadenas de datos, objetos  y funciones y se pueden referenciar con un nombre
Para declarar una variable en JavaScript se utilizan las palabras claves “var”, “let” o “const”.

## 10.	¿Qué es una biblioteca o framework de JavaScript y cuáles son algunos de los más populares?

R/ es un conjunto de herramientas, funciones y utilidades predeterminadas que facilitan el desarrollo de aplicaciones web.
Algunas bibliotecas son jQuery, lodash, momento.js
Y algunos framework angular, react,vue.js, ember.js, Svelte.

## 11.	¿Qué es un objeto en JavaScript y cómo se crea y utiliza?

R/ un objeto es una entidad que agrupa datos y funciones relacionadas en una sola unidad.
Un objeto en JavaScript está compuesto por pares clave-valor, donde las claves son cadenas (o símbolos) que actúan como nombres para acceder a los valores asociados. Estos valores pueden ser cualquier tipo de datos, como números, cadenas, booleanos, funciones u otros objetos. Además, las funciones dentro de un objeto se llaman métodos.
Hay varias maneras de crear un objeto una de las mas comunes es mediante la notación de objeto literal
// Objeto literal
const persona = {
  nombre: "Juan",
  edad: 30,
  esEstudiante: false,
  saludar: function() {
    console.log(`Hola, mi nombre es ${this.nombre} y tengo ${this.edad} años.`);
  }
};
Acceso a propiedades y métodos, agregar o modificar profesiones.

## 12.	¿Qué son los eventos en JavaScript y cómo se utilizan en una página web?

R/ Los eventos en JavaScript son interacciones o sucesos que ocurren en una página web, como hacer clic en un botón, mover el ratón sobre un elemento, presionar una tecla, cargar una página, entre otros. Los eventos permiten que el código JavaScript responda a las acciones del usuario o a cambios en el estado de la página.
Para capturar y manejar eventos en una página web, se utilizan manejadores de eventos. Estos son bloques de código (funciones) que se ejecutan en respuesta a un evento específico. Los manejadores de eventos permiten que tu código reaccione de manera dinámica a las acciones del usuario, lo que hace que las aplicaciones web sean interactivas y receptivas.
Aquí hay un ejemplo básico de cómo se utiliza un manejador de eventos para capturar el evento de clic en un botón:
HTML: ``<button id="miBoton">Haz clic</button>.``
javaScript: // Obtener referencia al elemento del botón
const boton = document.getElementById("miBoton");

// Agregar un manejador de evento para el clic
``boton.addEventListener("click", function() {
  alert("¡Botón clickeado!");
});.``
En este ejemplo, hemos utilizado el método addEventListener para vincular un manejador de evento al botón. Cuando el botón se hace clic, la función proporcionada se ejecuta y muestra un cuadro de alerta en el navegador.

## 13.	¿Qué son las peticiones HTTP y cómo se realizan en JavaScript?

R/ las peticiones HTTP son solicitudes que un cliente que generalmente es un navegador web envia para obtener, o enviar datos esta es la base de la comunicación entre navegador y servidor en la web.
En JavaScript, se pueden realizar peticiones HTTP utilizando la interfaz XMLHttpRequest o la más moderna API fetch(). Aquí te proporcionaré ejemplos de cómo se realizan peticiones HTTP utilizando ambas opciones.
// Crear un nuevo objeto XMLHttpRequest
``var xhr = new XMLHttpRequest();``

// Configurar la solicitud
``xhr.open("GET", "https://api.example.com/data", true);``

// Configurar un manejador de evento para la respuesta.


``xhr.onload = function() ``{
  ``if (xhr.status >= 200 && xhr.status < 300)`` {
    // La solicitud fue exitosa.
    ``console.log(xhr.responseText);``
  }`` else ``{
    // La solicitud falló
    ``console.error("Error en la solicitud:", xhr.statusText);``
  }
};

// Enviar la solicitud
``xhr.send();``

## 14.	¿Qué son los marcos de trabajo de front-end y cuáles son algunos de los más populares?

R/ son conjuntos de herramientas, bibliotecas y patrones de diseño que facilitan y agilizan el proceso de desarrollo de la interfaz de usuario y la lógica del lado del cliente en aplicaciones web. Estos marcos proporcionan una estructura organizada para construir aplicaciones web interactivas, dinámicas y receptivas.
Los mas populares son: React, Angular, Vue.js, Svelte,Ember.js,Mithril.

## 15.	¿Qué es una single-page application (SPA) y cómo se desarrolla utilizando JavaScript?

R/ Una Single-Page Application (SPA) es una aplicación web que funciona en una sola página HTML y carga dinámicamente el contenido necesario a medida que el usuario navega a través de la aplicación. En lugar de cargar páginas web completas cada vez que se realiza una acción, como hacer clic en un enlace, una SPA carga solo los datos y actualiza la vista en la página actual. Esto crea una experiencia de usuario más fluida y rápida, similar a una aplicación de escritorio.
Aquí hay una descripción general de cómo se desarrolla una Single-Page Application utilizando JavaScript:
1.	Estructura de la aplicación: En lugar de tener varias páginas HTML, una SPA generalmente tiene una única página HTML que sirve como contenedor para la aplicación. La mayoría del contenido de la aplicación se genera y actualiza dinámicamente mediante JavaScript.
2.	Enrutamiento: Una biblioteca o framework de enrutamiento (como React Router para React, Vue Router para Vue.js o Angular Router para Angular) se utiliza para manejar la navegación interna de la aplicación. Define rutas y componentes asociados para cada "página" lógica en la SPA.
3.	Componentes reutilizables: La aplicación se divide en componentes reutilizables, que son fragmentos de código que representan diferentes partes de la interfaz de usuario. Estos componentes se renderizan y actualizan dinámicamente a medida que el usuario interactúa con la aplicación.
4.	Manejo del estado: Se utiliza un sistema de manejo del estado (como Redux para React, Vuex para Vue.js o el enlace de datos de Angular) para administrar el estado de la aplicación y compartir datos entre los diferentes componentes.
5.	Comunicación con el servidor: Las SPAs a menudo utilizan peticiones AJAX (Asynchronous JavaScript and XML) o la API fetch() para comunicarse con un servidor y obtener datos. Los datos se actualizan en la interfaz de usuario sin recargar la página completa.
6.	Optimización de rendimiento: Dado que las SPAs pueden acumular una gran cantidad de JavaScript y datos, es importante implementar técnicas de optimización de rendimiento, como la carga diferida de recursos, la compresión de datos y la caché.



















