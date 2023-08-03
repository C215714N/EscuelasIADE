# Fundamentos WEB

Esto es una guia practica para los alumnos del curso de __Introduccion a HTML y CSS__, donde se recopilara informacion sobre los contenidos vistos durante las clases, ademas de ejercicios para poner en practica los temas tratados durante la capacitacion.

## Herramientas

Antes de continuar necesitaremos de un __editor de codigo__, _paciencia, actitud positiva y muchas ganas de aprender_.

Aqui dejo una lista de algunos editores que pueden utilizar para trabajar y algunas cositas a tener en cuenta con respecto a los mismos.

|Editor | Descripcion |
|--|--|
| [Visual Studio Code](https://code.visualstudio.com) | Perfecto para quienes empiezan en el mundo del desarrollo, instalas y listo para trabajar. |
| [Sublime Text](https://sublimetext.com) | Amigable con los desarrolladores, su interfaz es sencilla pero requiere ciertas nociones. |
| [Atom](https://atom.io) | Sus pantallas divididas son utiles para quienes usan sistemas de control de versiones. |
| [notepad++](https://notepad-plus-plus.org/) | Editor minimalista que requiere de poco espacio y bastante personalizable. |
| [Brackets](https://brackets.io) | Desarrollado con Javascript y pensado para ser utilizado por diseñadores web. |
| [VIM](https://www.vim.org/) | Para desarrolladores hardcore capaces de abandonar la GUI y concentrarse en el codigo. |

## Desarrollo frontend

En el mundo del __desarrollo web__ existen varias entidades que funcionan como reguladores del lenguaje, asi como referentes a la hora de escribir codigo, estableciendo lo que se conoce como __buenas practicas__.

> __W3C (World Wide Web Consortium)__ Encargada de definir el estandar y por lo tanto quien regula que elementos deben utilizarse y la sintaxis de los diferentes lenguajes web
>
> __WHATWG (Web Hypertext Application Technology Working Group)__ Fundada por _Mozilla y Apple_ se encarga de manetener y desarrollar HTML, ademas de las APIs para aplicaciones web.

Dentro de este mundo existe lo que se llama __Desarrollo FrontEnd__ que consiste en trabajar el codigo de la pagina web desde la Experiencia e interfaz de usuario, es decir, _el cliente_.

Se compone de aquellos lenguajes que pueden ser interpretados directamente por el navegador sin ninguna otra intervencion por parte del servidor y algunos de estos son:

* __HTML (Hypertext Markup Language)__ El lenguaje de marcado de hipertexto utiliza etiquetas para definir la funcion que cumple cada elementos dentro de la pagina, identificando asi la jerarquia de los mismos para facilitar a los motores de busqueda y al navegador su correcta interpretacion. Este aspecto se conoce como carga semantica y se utiliza para la indizacion de contenidos.
_ejemplo: `<p>parrafo</p>`_

* __CSS (Cascading Styles Sheets)__ Las hojas de estilo en cascada se utilizan para definir el diseño de los elementos representados en la pagina web, utilizando selectores y reglas para esto. El diseño debe planificarse en funcion de la estructura, teniendo en cuenta que este aspecto de la pagina esta destinado para mejorar la Experiencia de usuario mediante la interfaz.
_ejemplo: `p{color:blue;}`_

## Hojas de Estilo

Una vez definida la estructura de la pagina debemos pasar implementar el diseño de la misma, indicando a que elementos se les deben aplicar los cambios (selectores) y cuales seran los mismos, indicando el atributo a modificar, seguido de su valor (reglas)

> * *_estilo interno_* Es aquel que se utiliza dentro de la misma pagina
>	* *inline*: Es el mas facil de aplicar y tiene mayor prioridad, ya que debemos indicar a cada etiqueta sus cambios _e.g: `<div style="color: darkblue;">`_ siendo poco practico y lento.
>	* *inblock*: Es mas general que el anterior, pero los cambios aplicados solo funcionan dentro de la pagina, _e.g `div{ color: darkblue; }`_ pudiendo afectar a mas de una etiqueta a la vez, debido al selector.
> * *_estilo externo_* Es aquel que se implementa en un archivo aparte y asi utilizarlo en diferentes paginas, para poder vincularlo se coloca en la cabecera de pagina una etiqueta como la siguiente _`<link rel="stylesheet" href="styles.css">`_ indicando la ubicacion de la hoja de estilos.

## Formularios Web

Son herramientas que facilitan el intercambio de datos entre cliente y servidor mediante solicitudes HTTP (HyperText Tranfer Protocol) con la intervencion del usuario ya que es quien completa los datos a enviarse.

En un formulario encontraremos campos que indican que valores podemos ingresar. Las etiquetas correspondientes a los mismos son `<input>` para la mayoria de los campos monolinea, `<textarea>` para campos multilinea y `<select>` para listas de opciones; algunos de los tipo de datos mas comunes son:

|Tipo|Valor|
|----|----------|
|text | Cristian Racedo
|number|35336446|
|email|cristiandracedo@hotmail.com|
|password|******** |
| date|1991-04-18|
|radio|(O) masculino ( ) femenino|
|checkbox|[X] Español [X] Ingles [ ] Portugües |
|textarea | Descripcion del Perfil profesional <br> Experiencia Laboral y Habilidades|
|select| seleccione un lenguaje <br> html <br> css <br> js |

## Tablas 
Conjunto estructurado de datos distribuidos en filas y columnas __(tabulados)__, que permite buscar con rapidez y facilidad valores entre diferentes tipos de datos que indiquen algún tipo de conexión.

Cuando se hace correctamente, incluso las personas ciegas pueden interpretar los datos de una tabla HTML, ya que debe mejorar la experiencia de los usuarios videntes e invidentes por igual.

| ![Tabla Clasica](assets/docs/table.svg "Estructura Clasica") | ![Tabla Semantica](assets/docs/table_structure.svg "Estructura Semantica") |
|--|--|
| Clasica | Semantica |
___

## Actividades

En este apartado se podran realizar diferentes ejercicios relacionados con los temas dictados en clase, organizados por contenido y donde se pondra a prueba su experiencia en el mundo del desarrollo web.

### Conceptos Basicos
1. Realizar el tipo de lista que corresponda y ordenar, en caso que sea necesario, los siguientes elementos:
   * "edad media(3300 A.C. – 476 D.C)",  "edad antigua (476 – 1492)", "edad contemporanea (1789 – actualidad)", "edad moderna (1492 – 1789)"
   * "Futbol", "Tenis", "Rugbi", "Golf", "Beisbol", "Baloncesto", "Handball"
   * "Argentina", "Chile", "Bolivia", "Brasil", "Uruguay", "Paraguay"
   * "Casper Ruud(4960pts)", "Novak Djokovic (7595pts)", "Carlos Alcaraz (7675pts)", "Daniil Mendeleev (5890pts)", "Stefanos Tsitsipas(4670pts)"

### Estructura de un sitio
1. Crear una sitio web de al menos 3 paginas utilizando la estructura semantica.
2. En cada pagina debe haber un menu de navegacion permita desplazarnos entre las mismas, como por ejemplo:
   * [inicio](index.html)
   * [nosotros](about.html)
   * [galeria](gallery.html)
3. Diferenciar el `<header>` y `<footer>` utilizando un `color` y `background-color` a eleccion
4. Agregar hipervinculos de las redes sociales a eleccion e informacion de copyright
5. Colocar contenido dentro de las diferentes paginas a eleccion.

### Formularios
1. Crear un formulario de inicio de sesion utilizando los siguientes elementos
   * un campo de tipo __email__
   * un campo de tipo __password__.
2. Crear un formulario de registro que respete los siguientes criterios:
   * nombre y apellido __(obligatorio)__
   * fecha de nacimiento
   * telefono y celular
   * correo y contraseña __(obligatorio)__
3. Crear un formulario para una red social que posea:
   * campo para __nombre__
   * campo de __comentario__
   * opcion para elegir entre _publica o privada_.