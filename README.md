# Semana 5: HTML & CSS
Una introducción pragmática a HTML y CSS. Este curso está diseñado para los estudiantes amantes de aprender practicando y leyendo código. 

## Contenido
El curso está dividido en las siguientes secciones:

0. Prework. En internet se puede encontrar mucha información teórica sobre qué es HTML y qué es CSS. Usando como base el principio `Don't Repeat Yourself` no pretendemos tratar de definir con nuestras propias palabras qué es HTML y CSS. La definición puedes encontrarla tu mismo/a y discutir en clase con tus propias palabras: ¿Qué es y para qué sirven HTML & CSS?
1. Lenguajes de Marcado Parte 0
    1. HTML.
        1. p, b, a y h3.
        2. Cancionero 0.1.0
    2. CSS. 
        1. color, background, font inline.
        2. Cancionero 0.2.0
        3. Style tag
        4. Cancionero 0.3.0
        5. External files
        6. Cancionero 0.4.0
    3. Mark Down.
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
    3. Sass

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

### p, b, a y h

Las `tags`: `<p>`, `<b>`, `<a>` y `<h>` definen los siguientes elementos:
* Párrafos `<p>`
* Negritas `<b>`
* Enlaces `<a>`
* Encabezados (`headers`) `<h>`
### Cancionero

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
        <h1>Artista: Placebo</h1>
        <h2>Canción: Every You Every Me</h2>
        <p>
            Sucker love is heaven sent
            You pucker up our passion's spent
            My hearts a tart your body's rent
            My body's broken yours is bent
        </p>

        <p>
            Carve your name into my arm
            Instead of stressed I lie here charmed
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
