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

### Borrar palabra 

**Combo:** <kbd>d</kbd> + <kbd>e</kbd>.

**Ejemplo:**

Si tuviéramos el siguiente código:

```css
font-size: 13px 12px
```

Si situamos el cursor delante del palabra <kbd>12px</kbd> al aplicar el combo <kbd>de</kbd>, obtendríamos lo siguiente:

```css
font-size: 13px
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



----------


## Navegación

Explicación.

| Item     | Value | Qty   |
| :------- | ----: | :---: |
| Computer | $1600 |  5    |
| Phone    | $12   |  12   |
| Pipe     | $1    |  234  |
