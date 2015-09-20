# Vim key combinations

One of the most pleasant aspects of **Vim** is how **keyboard shortcuts** can be **combined**. In this
repository we will describe some of those combinations.

Uno de los aspectos más agradables de **Vim** es como sus **atajos de teclado** se pueden **combinar**. En
este repositorio describiremos algunas de esas combinaciones.

> **Note:**
> If you know any other **key combination**, please do not hesitate to make a **pull-request**.

> **Nota:**
> Si conoces alguna otra **combinación**, por favor no dudes en hacer un **pull-request**.



----------

## Modos


### Modo Insertar 

**Tecla:** <kbd>i</kbd>.

**Ejemplo:**

Si tuviéramos el siguiente código y posicionamos el cursor delante del caracter <kbd>S</kbd>:

```js
var order = 'SC';
```

Y luego presionamos la tecla <kbd>i</kbd> pasamos a modo inserción, luego escribimos por ejemplo la letra A, tendríamos:

```js
var order = 'ASC';
```

**Tecla:** <kbd>a</kbd>.

**Ejemplo:**

Si tuviéramos el siguiente código y posicionamos el cursor delante del caracter <kbd>D</kbd>:

```js
var order = 'DSC';
```

Y luego presionamos la tecla <kbd>a</kbd> pasamos a modo insersión, luego escribimos por ejemplo la letra E, tendríamos:

```js
var order = 'DESC';
```




----------

## 2 keys


### Cambiar de posición un caracter con el caracter siguiente 

**Combo:** <kbd>x</kbd> + <kbd>p</kbd>.

**Ejemplo:**

Si tuviéramos el siguiente código:

```js
var roder = 'ASC';
```

Si situamos el cursor delante del caracter <kbd>r</kbd> al aplicar el combo <kbd>xp</kbd>, obtendríamos lo siguiente:

```js
var order = 'ASC';
```


### Eliminar una línea de código entera 

**Combo:** <kbd>d</kbd> + <kbd>d</kbd>.

**Ejemplo:**

Si tuviéramos el siguiente código:

```css
p
    margin 0
    color white
```

Si situamos el cursor sobre <kbd>margin 0</kbd> al aplicar el combo <kbd>dd</kbd>, obtendríamos lo siguiente:

```css
p
    color white
```

### Borrar resto de palabra desde un punto específico 

**Combo:** <kbd>d</kbd> + <kbd>e</kbd>.

**Ejemplo:**

Si tuviéramos el siguiente código:

```css
box-sizingabc: border-box
```

Si situamos el cursor en el caracter <kbd>a</kbd> al aplicar el combo <kbd>de</kbd>, obtendríamos lo siguiente:

```css
box-sizing: border-box
```



### Ir hasta la primera línea de código de un archivo 

**Combo:** <kbd>g</kbd> + <kbd>g</kbd>.

**Ejemplo:**

Si tuviéramos el siguiente código:

```js
/*
GulpCssUrlVersioner
@class GulpCssUrlVersioner
 */

/*
 * Module dependencies.
 */
var Buffer, CssUrlVersioner, GulpCssUrlVersioner, chalk, extend, through, util;

util = require('util');
through = require('through2');
chalk = require('chalk');
Buffer = require('buffer').Buffer;
extend = util._extend;
CssUrlVersioner = require('css-url-versioner');

/*
 * Library.
 */
GulpCssUrlVersioner = function(opts) {
  this.data = {};
  this.settings = opts || {
    debug: false
  };
  this.css = '';
  this.transform();
  return this.stream;
};
```

y tuviéramos el cursor posicionado en cualquier línea, al aplicar el combo <kbd>gg</kbd>, el cursor se posicionaría delante del primer caracter de la primera línea de codigo de nuestro archivo.




### Ir hasta la última línea de código de un archivo 

**Tecla:** <kbd>G</kbd>.

**Ejemplo:**

Si tuviéramos el siguiente código:

```js
/*
GulpCssUrlVersioner
@class GulpCssUrlVersioner
 */

/*
 * Module dependencies.
 */
var Buffer, CssUrlVersioner, GulpCssUrlVersioner, chalk, extend, through, util;

util = require('util');
through = require('through2');
chalk = require('chalk');
Buffer = require('buffer').Buffer;
extend = util._extend;
CssUrlVersioner = require('css-url-versioner');

/*
 * Library.
 */
GulpCssUrlVersioner = function(opts) {
  this.data = {};
  this.settings = opts || {
    debug: false
  };
  this.css = '';
  this.transform();
  return this.stream;
};
```

Y tuviéramos el cursor posicionado en cualquier línea, al presionar la tecla <kbd>G</kbd>, el cursor se posicionaría en el último caracter de la última línea de código de nuestro archivo.




### Copiar y pegar una linea debajo de linea actual

**Combo:** <kbd>yy</kbd> + <kbd>p</kbd>.

**Ejemplo:**

Si tuviéramos el siguiente código:

```js
var a = "Test";
```

Si situamos el cursor en cualquier posición de la linea, al aplicar el combo <kbd>yyp</kbd>, obtendríamos lo siguiente:

```js
var a = "Test";
var a = "Test";
```



----------

## 3 keys

### Intercambiar la posición con la línea inferior

**Combo:** <kbd>d</kbd> + <kbd>d</kbd> + <kbd>p</kbd>.

**Ejemplo:** 

Si tuviéramos el siguiente código:

```css
p
    margin 0
    color white
```

Si situamos el cursor sobre <kbd>margin 0</kbd> al aplicar el combo <kbd>ddp</kbd>, obtendríamos lo siguiente:

```css
p
    color white
    margin 0
```

### Eliminar un grupo de caracteres (alfanumericas,caracteres especiales).

**Combo:** <kbd>c</kbd> + <kbd>a</kbd> + <kbd>w</kbd>.

**Ejemplo:** 

Si tuviéramos el siguiente código:

```css
h1
    color red
```

Si situamos el cursor sobre el atributo <kbd>color</kbd>, y ejecutamos el combo en modo normal, obtendríamos lo siguiente:
```css
h1
    red
```


----------


## Navegación

Explicación.

| Item     | Value | Qty   |
| :------- | ----: | :---: |
| Computer | $1600 |  5    |
| Phone    | $12   |  12   |
| Pipe     | $1    |  234  |
