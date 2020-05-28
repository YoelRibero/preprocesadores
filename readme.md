# Introducción

_Curso de pre-procesadores de Platzi. Elabora la estructura de las páginas de un sitio web utilizando PUG. Define los estilos de cada página implementando Less, Sass y Stylus. Utiliza funciones, variables y condicionales para reutilizar código y organizarlo de manera óptima._

### Conceptos Básicos

_CSS significa **Cascading Style Sheets** o su traducción al español Hojas de Estilo en Cascada._

Asignar reglas CSS a un documento HTML se puede hacer de varias formas:

- Colocando las reglas en un documento `*.css` y relacionarlo al HTML usando la etiqueta
- Colocando en el atributo `style` de cada elemento HTML las reglas para cada etiqueta.
- Colocando los estilos dentro de una etiqueta `style` dentro del `head` del documento.

Como su nombre lo dice siempre lee en cascada de arriba hacia abajo sobrescribiendo valores excepto los dados por el atributo `style`.

**Un estilo CSS está formado por: selector, declaración, propiedad y valor.**

### Selectores

_Los selectores nos sirven para seleccionar los diferentes elementos en una página web y aplicar estilos._

Existen los siguientes tipos de selectores:

- **Selector universal:** Sirve para agregar estilos a todos los elementos de la página. Normalmente se utiliza para hacer “reset” de estilos.
- **Selector etiqueta:** Aplica estilos a todos los elementos de ese tipo (p, h1, header etc.).
- **Selector id:** Aplica estilos a un elemento único con ese Id, se recomienda hacer buen uso de este selector.
- **Selector clase:** Aplica estilos a todos los elementos con esa clase (el que más vas a usar).
- **Selector anidado:** Aplica estilos a un elementos descendientes de otros elementos (no necesario que sea hijo directo).
- **Selector hijo > :** Aplica estilos a los elementos que sean hijos directos de otros.
- **Selector adyacente + :** Aplica estilos al elemento adyacente.
- **Selector de atributo input[type=“number”] :** Aplica estilos al elemento con el atributo especificado.

La prioridad de un selector se determina por la suma de su contenido:

- ID = 100
- Clase = 10
- Etiqueta = 1

A mayor la suma, mayor prioridad.

**!important** es un valor especial tiene un valor de un millón, nunca usar a menos que sea tu única opción como cuando no tienes acceso al código fuente.

### Pre-Procesadores

Es una herramienta que permite escribir pseudocódigo que luego será convertido a css o HTML standard.

Extiende el poder de CSS y HTML al nivel de un lenguaje de programación más potente con características tales como variables, funciones y mixins.

### Metodologías para esctructurar código

_Las metodologías para estructurar código son sistemas preestablecidos, formales y bien documentados, que te ayudan a escribir y organizar código mantenible y escalable en sistemas grandes y complejos._

Las métodologías son:

- **SMACSS**
- **BEM**
- **Atomic CSS**
- **OOCSS**

### Metodología BEM

_BEM es la metodología que vamos a usar a lo largo del curso. El objetivo de BEM es dividir lógicamente las piezas de las que se compone una web._

BEM establece que debemos usar clases para nuestro selectores, clases que se dividen en:

- **Bloques:** Los bloques son nuestros contenedores más grandes que a su vez contienen elementos u otros bloques.
- **Elementos:** Los elementos siempre forman parte de un bloque, normalmente son los botones, textos, imágenes etc.
- **Modificadores** Los modificadores se usan para establecer estilos diferentes a un mismo bloque o elemento.

##### Sintaxis

- `.bloque{}`
- `.bloque_elemento{}`
- `.bloque--modificador{}`

Ejemplo:

- `.galeria{}`
- `.galeria_foto{}`
- `.galeria_foto--circular{}`

### Guías para la cración y mantenimiento de código

_La meta de tener una guía de código es hacer que luzca como si una sola persona lo haya escrito para que se entendible por todo el equipo._

Para el proyecto **PlatziGames** tenemos una guía en la que definimos:

- Ser consistentes con la indentación.
- Consistencia con espacios, corchetes, puntos y comas.
- Consistencia de números, de selectores y divisiones.
- Agrupaciones de propiedades.
- Uso de ID’s y clases.

[Guía de código](https://static.platzi.com/media/public/uploads/guia-de-codigo-platzi-games_f19c63bf-af70-4aeb-8ac1-3e905bc140ab.pdf)
