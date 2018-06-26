# Semana 5: HTML & CSS
Una introducción pragmática a HTML y CSS. Este curso está diseñado para los estudiantes amantes de aprender practicando y leyendo código. 

## Contenido
El curso está dividido en las siguientes secciones:

0. Prework. En internet se puede encontrar mucha información teórica sobre qué es HTML y qué es CSS. Usando como base el principio `Don't Repeat Yourself` no pretendemos tratar de definir con nuestras propias palabras qué es HTML y CSS. La definición puedes encontrarla tu mismo/a y discutir en clase con tus propias palabras: ¿Qué es y para qué sirven HTML & CSS?
1. [Lenguajes de Marcado Parte 0](#lenguajes-de-marcado-parte-0)
    1. [HTML](#html).
        1. p, b, a y h3.
        2. Cancionero 0.1.0
    2. [CSS](#css). 
        1. color, background, font inline.
        2. Cancionero 0.2.0
        3. Style tag
        4. Cancionero 0.3.0
        5. External files
        6. Cancionero 0.4.0
    3. [Markdown](#markdown).
2. Lenguajes de Marcado Parte 1
    1. Utilizamos CSS existente
        1. Compañeros a Colegas.
    2. Listas
        1. Tu primer lista
        2. Cancionero 0.6.0
    3. Tablas
        1. Tu primer tabla
        2. Cancionero 0.5.0
        3. Estilo en tablas
        4. Cancionero 0.6.0
    4. Divs
        1. Tus primeros divs
        2. Propiedades comunes de los divs.
        3. Cancionero 0.7.0      
3. Lenguajes de Marcado Parte 2
    1. HTML5
    2. CSS3
    3. [Sass](https://www.sassmeister.com/)

4. Bulma
    1. Introducción a Bulma
      1. Proyecto base
      2. Cancionero 0.8.0
5. Lenguajes de Marcado Parte 3
    1. Formularios
    2. iFrames
6. Github
    1. Github pages
    2. Crea tu página en github.
7. Git
    1. Commits, remotes
    2. Sube tus cambios a github
8. CV Online
  
## Lenguajes de Marcado Parte 0
### HTML
HTML se categoriza como un lenguaje de marcado. Este tipo de lenguajes códfican un documento con etiquetas (`tags`) que contienen información adicional de la estructura del texto que contienen y su presentación. Un documento es considerado html cuando su extensión así lo indique y cuando su contenido siga la siguiente estructuctura básica:
```html
<html>
    <head></head>
    <body>
    </body>
</html>
```

A las palabras que se encuentran dentro de los siguientes sigons `<` `>` como `<body>` y `<head>` se les conoce como etiquetas o `tags`. De ahora en adelante nos referiremos a estos elementos como `tags`.

Existe una gran cantidad de etiquetas disponibles para usarse en cualquier documento html. Si quieres conocerlas todas te recomiendo que leas la documentación de cada una en [w3schools](https://www.w3schools.com/Html). En este curso abarcaremos las más fundamentales explicadas a continuación.

#### p, b, a y h

Las `tags`: `<p>`, `<b>`, `<a>` y `<h>` definen los siguientes elementos:
* Párrafos `<p>`
* Negritas `<b>`
* Enlaces `<a>`
* Encabezados (`headers`) `<h>`
#### Cancionero

Para practicar con las etiquetas mencionadas vamos a crear un Cancionero.
¿Cuál es tu banda o artista favorito? ¿Cuál es tu canción favorita de este artista? Ya la tienes, bueno ahora sí, ¡Manos en la computadora!

1. Crea un documento html. Desde una terminal (ó cmd) crea el archivo cancionero:
```bash
touch cancionero.html
```
2. Abreló, agrega la siguiente estructura y guarda los cambios:
```html
<html>
    <head>
        <title>Placebo</title>
    </head>
    <body>
        <h1>Artista: <a href="https://es.wikipedia.org/wiki/Placebo_(banda)">Placebo</a></h1>
        <h2>Canción: Every You Every Me</h2>
        <p>
            Sucker love is heaven sent
            You pucker up our passion's spent <br>
            My hearts a tart your body's rent
            My body's broken yours is bent
        </p>

        <p>
            Carve your name into my arm
            Instead of stressed I lie here charmed <br>
            Cause there's nothing else to do
            Every me and every you
        </p>

        <p>
          Sucker love a box I choose
          No other box I choose to use
          Another love I would abuse
          No circumstances could excuse  
        </p>
        <p>
            In the shape of things to come
            Too much poison come undone
            Cause there's nothing else to do
            Every me and every you
            Every me and every you
            Every me
        </p>
        <p>
           Sucker love is known to swing
           Prone to cling and waste these things
           Pucker up for heavens sake
           There's never been so much at stake 
        </p>
        <p>
            I serve my head up on a plate
            It's only comfort, calling late
            Cause there's nothing else to do
            Every me and every you
            Every me and every you
            Every me,
        </p>
    </body>
</html>
```
3. Remplaza respectivamente mi artista favorito, mi canción favorita y la letra de mi canción por los tuyos.
4. Abre el archivo en tu navegador Chrome ;)
#### Attributos HTML

Los atributos son usados para agregar información adicional a cada `tag`. Los atributos más usados son:
* href
* src
* width y height
* alt
* style

Algunos `tags` html solo hacen sentido si tienen un atributo especificado, por ejemplo el tag `<a>`:
```html
<a href="https://es.wikipedia.org/wiki/Placebo_(banda)">Placebo</a>
```
En este caso el `tag` `<a>` necesita del atributo `href` para poder redireccionar a la página en wikipedia de placebo.

#### Cancionero 0.2.0
Vamos a prácticar el con los atributos HTML. Para esto agreguemos atributos nuevos al `tag` `<a>`.
```html
<h1>
    Artista:
    <a  href="https://es.wikipedia.org/wiki/Placebo_(banda)"
        alt="Ir a Placebo en Wikipedia"
        target="_blank"
        style="color:red"
        >
        Placebo
    </a>
</h1>
```
### CSS
Es un lenguaje usado para descibir cómo se mostrará cada `tag` dentro de un documento HTML. Aunque también puede utilizarse para descrbir otros documentos de marcado, como XML o XHTML, CSS es usado principalmente con HTML.

Una primera aproximación a CSS puede hacerse agregando o modificando el atributo style de cada elemento, así como lo hicimos en el ejercicio anterior con el atributo `<a>`:
```html
    <a  href="https://es.wikipedia.org/wiki/Placebo_(banda)"
        alt="Ir a Placebo en Wikipedia"
        target="_blank"
        style="color:red"
        >
        Placebo
    </a>
```
#### color, background, font
Ahora veremos cómo modificar tres propiedades fundamentales que dan estilo a cualquier `tag` html: [color](https://www.w3schools.com/css/css_colors.asp), [background](https://www.w3schools.com/css/css_background.asp) y [font](https://www.w3schools.com/css/css_font.asp) (si quieres conocer más de cada una solo da clic).

Seguiremos trabajando con el elemento `<a>`:
```html
    <a  href="https://es.wikipedia.org/wiki/Placebo_(banda)"
        alt="Ir a Placebo en Wikipedia"
        target="_blank"
        style="color:tomato; background-color: gray; font-family: 'Lucida Console'; font-style: italic; font-size: 40px"
        >
        Placebo
    </a>
```
#### Cancionero 0.3.0

1. Modifica el cancionero para que cada parrafo tenga una imagen de fondo diferente.
2. Agrega a cada parrafo para que la letra se distinga del fondo.
3. Cada parrafo debe tener un tamaño de font diferente.

#### Style
Hasta ahorita hemos utilizado CSS dentro del atributo *style* de cada uno de nuestros `tags`, a esta forma de declarar el estilo se le denomina *inline* y aunque es la forma más sencilla de utilizar css tambien es la menos mantenible (o más cochina).

El código CSS añadido a cada selector puede separarse en un `tag` HTML llamado `<style>`. Por ejemplo si queremos cambiar el color del body agregamos lo siguiente dentro de la etiqueta `<head>`:
```html
<head>
    <title>Placebo</title>
    <style>
    body {
        background-color: black;
    }
    </style>
</head>
```
Ahora nos damos cuenta que las letras no se ven ¿cómo podemos solucionar el problema para que se vean las letras?

#### Cancionero 0.4.0

1. Modifica el códgio del cancionero para que los estilos se definan dentro de la etiqueta `<style>`

#### Archivos externos

El `tag` `<link>` se utiliza para poder enlazar archivos externos. Principalmente lo usamos para poder enlazar documentos CSS o *Javascript* a nuestro documento HTML. 

#### Cancionero 0.5.0
1. Copia todo lo que pusiste dentro de la etiqueta `<style>` y pegalo en un archivo con extensión css. El archivo debe llamarse: `style.css`
```css
body {
    background-color: black;
    color: white;
}

p {
    text-align: left;
    text-indent: 15px;
}

h1 {
    color: blue;
    text-transform: uppercase;
}

a:hover {
  color: yellow;
}

```
2. Enlaza el documento CSS a nuestro documento HTML.
```html
<head>
    <link rel="stylesheet" href="style.css">
</head>
```
3. Modifica el estilo de tu cancionero ;)

### Markdown

Mark Down es otro tipo de lenguajes de marcado. No es necesario para hacer páginas web pero se ha convertido en uno de los más utilizados para escribir en internet. Puedes ver el siguiente enlace con una lista de comandos básicos: [Markdown Cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet) que puedes práciticar en este sitio web: http://markdownlivepreview.com/. Te reto a que escribas tu canción favorita en Markdown ;)

## Lenguajes de Marcado Parte 1
Ahora que sabemos lo básico de HTML y CSS vamos a continuar aprendiendo nuevos `tags` de HTML y propiedades CSS.

### Compañeros a colegas

Como vimos en el capítulo pasado, podemos usar un archivo CSS para que nuestro HTML se vea bonito <3. Pide a tu compañero que te comparta su archivo `style.css` para que lo uses en tu proyecto Cancionero.

### Listas

Ahora vamos a utilizar el `tag` `<ul>`, tambien conocido como lista.

```html
<h1>Lista de Canciones</h2>
<ul>
    <li>Pure morning</li>    
    <li>The Bitter End</li>
</ul>
```

### Tablas

Una tabla es un selectior que se usa comunmente en páginas HTML. Muchas personas lo usaban para dar un formato a la página web, sin embargo esto ha ido cambiando y ahora solo se usan para mostrar información.

```html
<table>
    <tr>
        <th>Canción</th>
        <th>Album</th>
    </tr>
    <tr>
        <td>Pure Morning</td>
        <td>Without You I'm Nothing</td>
    </tr>
    <tr>
        <td>The Bitter End</td>
        <td>Sleeping with Ghosts/td>
    </tr>
</table>
```

## Divs
Los `tags` `<div>` son bloques HTML que se utilizan como contenedores de otros `tags`. Por lo tanto, se usan para formar una estructura dentro de un HTML.

Por ejemplo si quisieramos mostrar la lista de canciones de placebo, utilizadas anteriormente, utilizaríamos una estructura html de la siguiente forma.

```html
<html>
    <head></head>
    <body>
        <div>
            <div>
                <h1>
                <span>Artista:</span>
                <a  href="https://es.wikipedia.org/wiki/Placebo_(banda)"
                        alt="Ir a Placebo en Wikipedia"
                        target="_blank"
                        style="color:tomato; background-color: gray; font-family: 'Lucida Console'; font-style: italic; font-size: 40px"
                        >
                        Placebo
                    </a>
                </h1>
            </div>
            <div>
                <h2>Canción: Every You Every Me</h2>
            </div>
            <div>
                <!--Aqui va la letra de la cancion--->
            </div>
        </div>
    </body>
</html>
```

`<span>` es otro `tag` de tipo bloque, solo que es considerado `inline` esto quiere decir que el contenido debería consistir de no más de una línea.

De momento no se muestra un cambio visual drástico, sin embargo ya tenemos un documento mejor estructurado sobre el cuál podremos realizar manipulaciones de estilo... por el momento.

### Divs con estilo

Ahora que conocemos cómo funcionan los `divs` vamos a trabajar en sus propiedades CSS para hacerlo más atractivo.

```css
div {
  background-color: black;
  color: white;
  text-align: center;
  font-size: 20px;
  border-color: blue;
  border-style: solid;
  border-width: 5px;
}
```
```html
<div>
  <p>
    Placebo    
  </p>
</div>
<div>
  <p>
    Song to Say Goodbye - Meds
  </p>
</div>
```

¿Como podemos hacer para que cada div tenga atributos diferentes? Por ejemplo, que el tamaño de la letra del título de la canción sea diferente.

#### Ids

El lenguaje css está compuesto de selectores y las propiedades de cada selector. Un selector hace referencia a un elemento HTML. Por ejemplo, el siguiente selector hace referencia al tag `<div>`:

```css
div {
  background-color: black;
  color: white;
  text-align: center;
  font-size: 20px;
  border-color: blue;
  border-style: solid;
  border-width: 5px;
}
```

Si queremos identificar un div espécifico debemos agregar el atributo `id` a cada tag que querramos identificar. Por ejemplo:

```html
<div id='artist'>
  <p>
    Placebo    
  </p>
</div
```

Una vez tengamos identificado el `tag` podemos usar su id como identificador en nuestro css:
```css
#artist {
    font-size: 40px;
}
```

#### Classes
Las *classes* nos sirven para poder identificar un conjunto de elementos dentro de un HTML, a diferencia de los *ids* en donde solo podemos identificar uno.

```css
.lyrics {
    font-size: 16px;
    font-style: italic;
}
```

```html
<div>
  <p class="lyrics">
    A song to say goodbye
  </p>
  <p class="lyrics">
    Lara Lara
  </p>
</div>
```
