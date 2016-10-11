![jointDeveloper](https://raw.githubusercontent.com/jointDeveloper/Aprendizaje-Web/gh-pages/IMG/robot-logo.png)

# Comunidad jointDeveloper

## Distribución
```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <link rel="stylesheet" href="css/style.css">
    <title>Portafolio</title>
  </head>
  <body>
    <header></header>
    <main></main>
    <footer></footer>
  </body>
</html>

```
```css
* {box-sizing: border-box; }

html, body {
  height: 100%;
  margin: 0;
  padding: 0;
  width: 100%;
}
```
### Letra/Fuente
_Referencia: [Google Fonts](https://fonts.google.com/)_

* e.g. Architects Daught
```html
<head>
  ...
  <link href="https://fonts.googleapis.com/css?family=Architects+Daughter" rel="stylesheet">
  ...
</head>
```
```css
html, body {
  font-family: 'Architects Daughter', cursive;
  ...
}
```
___
## Barra de Navegación/NavBar
```html
<header>
  <nav>
    <ul>
      <li><a href="#intro">Alejandro E. Rendon</a></li>
      <li><a href="#bio">Bio</a></li>
      <li><a href="#portafolio">Portafolio</a></li>
      <li><a href="#contacto">Contacto</a></li>
    </ul>
  </nav>
</header>
```

```css
nav {
  background-color: white;
  box-shadow: 0 2px 10px black;
  color: black;
  font-weight: bold;
  position: fixed;
  text-align: center;
  width: 100%;
}

nav > ul {
  height: 60px;
  margin: 0;
  padding: 0;
  list-style: none;
}

nav > ul > li {
  display: inline-block;
  padding: 18px;
}

nav > ul > li:hover {
  background-color: black;
  color: white;
  opacity: 0.5;
}

a {
  text-decoration: none;
}
```
___
## Contenido
1. Introducción/Presentación
2. Biografía
3. Portafolio
4. Contacto `<footer>`

```html
...
<main>
  <div class="content" id="intro">
    <h1>Alejandro E. Rendon</h1>
  </div>
  <div class="content" id="bio">
    <h1>Bio</h1>
  </div>
  <div class="content" id="portafolio">
    <h1>Portafolio</h1>
  </div>
  <div class="content" id="contacto">
    <h1>Contacto</h1>
  </div>
</main>
...
```
```css
main {
  height: 100%;
  width: 100%;
}

.content {
  min-height: 100%;
  padding: 50px 30px;
  text-align: center;
  width: 100%;
}
```
### 1. Introducción

#### Fondo
##### Color
```css
#intro { background-color: #009c41; }
```
##### Imágen
```css
#intro {
  background-image: url(../img/fondo.jpg);
  background-repeat: no-repeat;
  background-size: cover;
}
```

#### Imagen del Perfil
Colocar la imagen de perfil en el directorio `/img` y se agrega con la etiqueta `<img>` en la sección.

```html
<div class="content" id="intro">
  <img src="img/foto.png" alt="Foto de perfil" />
  ...
</div>
```
Algunos detalles visuales para la imagen:
```css
#intro > img {
  border-radius: 50%; /* Bordo Redondeado */
  height: 200px;
  width: 200px;
}
```
#### Más Información (Vínculos, Redes Sociales, etc.)

Para agregar por ejemplo la información de redes sociales, se pueden utilizar iconos con vínculos. Por lo general como estandar se agregan los iconos o imagenes al directorio `img/icons/`

Para crear un vínculo o enlace con una imagen, basta con la siguiente línea de código
```html
<a href="Dirección/URL"><img src="img/icons/nombre_icono.png" /></a>
```
e.g.
```html
<div class="content" id="intro">
  ...
  <div id="informacion">
    <a href="http://www.facebook.com"><img src="img/icons/facebook.png" /></a>
  </div>
</div>
```
_Nota: Algo común en los enlaces externos es que se abran en una pestaña diferente en el navegador, para esto solo es necesario agregar el atributo `target="_blank"` dentro del tag `<a>`_ i.e.
```html
<a href="http://www.facebook.com" target="_blank"><img src="img/icons/facebook.png" /></a>
```
Algo de estilo visual para los iconos
```css
#informacion > a > img {
  height: 60px;
  width: 60px;
}
```
```css
#informacion > a > img:hover {
  opacity: 0.5;
}
```
## Biografía



___
## Algunos Enlaces de Interés
* _[Colores con Código RGB](http://www.flatcolorsui.com/)_
* _[Iconos](http://www.flaticon.com/)_
