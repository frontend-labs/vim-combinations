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

## Movimiento del Cursor(Desplazamiento)

### Saltar hacia el inicio de una línea

**Tecla:** <kbd>0</kbd>.

**Ejemplo:**

Si tuviéramos el siguiente código y tenemos el cursor en cualquier posición:

```js
var order = 'ASC';
```

Y luego presionamos la tecla <kbd>0</kbd> el cursor se desplazará hacía el inicio de la línea, osea el cursor se pondrá delante de la letra <kbd>var</kbd>.


### Modo Normal o Modo Navegación

Este modo de vim es el que te permitirá navegar por todo el documento de una forma increíble. A este modo se accede presionando la tecla <kbd>Esc</kbd>.

En la siguente tabla mostramos la navegacion básica en vim: 

| Tecla     | Acción                                    |
| :-------- | :-----------------------------------      |
| k         | mueve el cursor hacia una línea superior. |
| j         | mueve el cursor hacia una línea inferior. |
| h         | mueve el cursor hacia un caracter a la izquierda |
| l         |  mueve el cursor hacia un caracter a la derecha |




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

### Deshacer el último cambio

**Tecla:** <kbd>u</kbd>.

----------

## 2 keys

### Rehacer el último cambio

**Tecla:** <kbd>Ctrl</kbd> + <kbd>R</kbd>.

### Comentar un bloque de líneas

Para aplicar este combo primero entrar al modo bloque visual.

**Combo:**<kbd>shift</kbd> + <kbd>i</kbd>.

**Ejemplo:**

Si tuviéramos el siguiente código:

```js
var a = 'SFSSD';
var b = 'SFSFSDFS';
var c = 'SFDSFDSFDSF';
```
Si situamos el cursor en la palabra reservada <kbd>var</kbd>, luego entrar al modo bloque visual, luego moverte hasta la linea que deseas comentar, en este caso sera <kbd>var</kbd> de la tercera linea , siempre posicionando en el primer caracter de la linea, luego aplicamos <kbd>shift</kbd> + <kbd>i</kbd> , luego <kbd>//</kbd> para comentar, luego <kbd>ESC</kbd> y listo.

```js
var a = 'SFSSD';
var b = 'SFSFSDFS';
var c = 'SFDSFDSFDSF';
```

Obtendremos :

```js
//var a = 'SFSSD';
//var b = 'SFSFSDFS';
//var c = 'SFDSFDSFDSF';
```

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

### Borrar resto de línea desde un punto específico 

**Combo:** <kbd>d</kbd> + <kbd>$</kbd>.

**Ejemplo:**

Si tuviéramos el siguiente código:

```css
border 1px 2px 3px 4px
```

Si situamos el cursor detrás de la palabra <kbd>2px</kbd> al aplicar el combo <kbd>d$</kbd>, obtendríamos lo siguiente:

```css
border 1px 2px
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

