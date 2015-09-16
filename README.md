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

[TOC]

----------


## Navegación

Explicación.

| Item     | Value | Qty   |
| :------- | ----: | :---: |
| Computer | $1600 |  5    |
| Phone    | $12   |  12   |
| Pipe     | $1    |  234  |

----------

## 2 keys

<kbd>d</kbd> and <kbd>d</kbd>

----------

## 3 keys

### Intercambiar la posición con la línea inferior

Combo: <kbd>d</kbd>, <kbd>d</kbd> y <kbd>p</kbd>

Si tuviéramos el siguiente código:

``css
// Example
p
    margin 0
    color white
``

Si situamos el cursor sobre <kbd>margin 0</kbd> al aplicar el combo <kbd>ddp</kbd>, obtendríamos lo siguiente:

``css
// Example
p
    color white
    margin 0
```

