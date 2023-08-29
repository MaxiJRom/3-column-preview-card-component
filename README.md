# baby MARKDOWN, MARKDOWN 🎵

1. [Formato de texto](#formato-de-texto)

1. [Código en linea y bloque de codigo](#código-en-linea-y-bloque-de-codigo)

1. [Encabezados](#encabezados)

1. [Citas](#citas)

1. [Listas](#listas)

1. [Columnas](#columnas)

1. [Agregar códigos en linea](#código-en-linea)

1. [Agregar bloques de código](#bloques-de-codigo)

1. [Comentarios y escape de carácteres](#comentarios-y-escape-de-carácterers)

1. [Insertar Links](#agregar-links)

1. [Insertar imágenes](#insertar-imagenes)

1. [Crear tabla de contenidos](#crear-tabla-de-contenidos)

## Formato de texto

\_\_negrita\_\_ ---> **negrita** <br>
\*\*negrita\*\* (recomendado)---> **negrita**

\_cursiva\_ --> _cursiva_ <br>
\*cursiva\* (recomendado)--> _cursiva_

\_\_\_negrita y cursiva\_\_\_ --> **_negrita y cursiva_** <br>
\*\*\*negrita y cursiva\*\*\* (recomendado)--> **_negrita y cursiva_**<br>
\*\*\_negrita y cursiva\_\*\* --> **_negrita y cursiva_**

<br>

Seguir el parrafo en el `[space][space] o <br>`  
renglón inferior sin que haya interlineado tan grande

Segun las buenas practicas de markdown es mejor poner la etiqueta de line break `<br>` <br>al final del parrafo

<br>

## Encabezados

# Encabezado de nivel 1

## Encabezado de nivel 2

### Encabezado de nivel 3

<br>

## Citas

> cita en un renglón

> cita en `[space][space] o <br>`  
> bloque

<br>

## Listas

    - lista  
    - desordenada

Output:
- lista  
- desordenada

---

    1. lista  
    1. ordenada

Output:
1. lista  
1. ordenada

---

    1. lista  
        - anidada  
            1. hola
                - buongiorno  
            1. ciao

Output:
1. lista  
    - anidada  
        1. hola
            - buongiorno  
        1. ciao
        1. domani

<br>

## Columnas

| Columna 1 | Columna 2 | Columna 3 |
| --------- | --------: | :-------: |
| A         |         B |     C     |
| D         |         E |     F     |
| G         |         H |     I     |

| Columna 1 | Columna 2 | Columna 3 |
| --------: | --------- | :-------: |
|         A | B         |     C     |
|         D | E         |     F     |
|         G | H         |     I     |

<br>

## Código en linea

- ssssssssssssssssssssssssssssssssssss `porcion de código en linea(alt  + 96 para el acento grave)` sssssssssssssssssssssssssssssssssssssssssssssssssssssssss

## Bloques de codigo

-     Dejando 4 espacios al ppio, se pone asi resaltado

- \```
  Tambien se pueden agregar porciones  
  de código en bloque  
  agregando 3 backticks antes y después del  
  codigo  
  \```

Output:

```
Tambien se pueden agregar porciones
de código en bloque
agregando 3 backticks antes y después del
codigo
```

- _El markdown interpreta código HTML:_

        <form>
        <label for="q">Buscar:</label>
        <input type="search" name="q" id="q" required  placeholder="que querei buscar"/>
        <input type="submit" value="🔍" />
        </form>

  Output:<br>
    <form>
    <label for="q">Buscar:</label>
    <input type="search" name="q" id="q" required  placeholder="que querei buscar"/>
    <input type="submit" value="🔍" />
    </form> <br><br>

- _Para otros lenguajes, se puede especificar de cual se trata para que lo muestre en colores:_

              ```js
          function sumar(a, b) {
          if (typeof a !== "number" || typeof b !== "number") {
              console.error(`Los valores ingresados NO son números.`);
              return false;
          }

          let c = a + b;
          return c;
          }
          ```

  Output:

  ```js
  function sumar(a, b) {
    if (typeof a !== "number" || typeof b !== "number") {
      console.error(`Los valores ingresados NO son números.`);
      return false;
    }

    let c = a + b;
    return c;
  }
  ```

  <br>

## Comentarios y escape de carácterers

    <!-------------- Asi se escriben comentarios---------->

<!-------------- Asi se escriben comentarios---------->

    \*\* la barra invertida provoca escape de carácteres, sino esto estaria en negrita \*\*

<br>

## Agregar links:

1.  Usando \[nombre a mostrar](link "texto hover")<br>

        [Mi perfil de GitHub](https://github.com/MaxiJRom "Ir al perfil")

    Output:  
    [Mi perfil de GitHub](https://github.com/MaxiJRom "Ir al perfil")

1.  Para transformar texto en linea en hipervínculos, encerrarlo en \<>: <br>

        "Aqui tiene un link para acceder a <https://www.google.com>"

    Output:<br>
    "Aqui tiene un link para acceder a <https://www.google.com>"

1.  Crear enlaces con estilo referencia:<br>

        Puede ser muy útil cuando se quiere ingresar un hipervínculo sin tener que agregar un URL horrible en el markdown, haciendolo ilegible.

        En lugar de esto:

            ```
            In a hole in the ground there lived a hobbit. Not a nasty, dirty, wet hole, filled with the ends
            of worms and an oozy smell, nor yet a dry, bare, sandy hole with nothing in it to sit down on or to
            eat: it was a [hobbit-hole](https://en.wikipedia.org/wiki/Hobbit#Lifestyle "Hobbit lifestyles"), and that means comfort.
            ```

        Escribimos esto:

        ```
        In a hole in the ground there lived a hobbit. Not a nasty, dirty, wet hole, filled with the ends
        of worms and an oozy smell, nor yet a dry, bare, sandy hole with nothing in it to sit down on or to
        eat: it was a [hobbit-hole][1], and that means comfort.


        [1]: <https://en.wikipedia.org/wiki/Hobbit#Lifestyle> "Hobbit lifestyles"
        ```
        Output:
        In a hole in the ground there lived a hobbit. Not a nasty, dirty, wet hole, filled with the ends
        of worms and an oozy smell, nor yet a dry, bare, sandy hole with nothing in it to sit down on or to
        eat: it was a [hobbit-hole][1], and that means comfort.

        [1]: <https://en.wikipedia.org/wiki/Hobbit#Lifestyle> "Hobbit lifestyles"

    <br>

## Insertar imagenes

    ![alt-img](url o ruta local img)

![Metabee](https://images-wixmp-ed30a86b8c4ca887773594c2.wixmp.com/f/72bec1c6-db33-455b-88f0-4fc53a7f9429/d2v4pnp-9804869c-1eaf-467d-b2d3-2fa8eb52ee2d.jpg/v1/fit/w_750,h_525,q_70,strp/metabee__10_by_adzstitch_d2v4pnp-375w-2x.jpg?token=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJzdWIiOiJ1cm46YXBwOjdlMGQxODg5ODIyNjQzNzNhNWYwZDQxNWVhMGQyNmUwIiwiaXNzIjoidXJuOmFwcDo3ZTBkMTg4OTgyMjY0MzczYTVmMGQ0MTVlYTBkMjZlMCIsIm9iaiI6W1t7ImhlaWdodCI6Ijw9NTI1IiwicGF0aCI6IlwvZlwvNzJiZWMxYzYtZGIzMy00NTViLTg4ZjAtNGZjNTNhN2Y5NDI5XC9kMnY0cG5wLTk4MDQ4NjljLTFlYWYtNDY3ZC1iMmQzLTJmYThlYjUyZWUyZC5qcGciLCJ3aWR0aCI6Ijw9NzUwIn1dXSwiYXVkIjpbInVybjpzZXJ2aWNlOmltYWdlLm9wZXJhdGlvbnMiXX0.2uEGvOirR8XRJobk7MQJXIc48XXRiRBrmob0tARPWU4)

## Se pueden hacer enlaces de las imagenes:

`[![alt-img](url-img)](url-enlace "titulo hover")`

    [![YouTube](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSWhfZCLVtXGkawxt6C2XjU4pAFQbQEOCc3cw&usqp=CAU)](https://www.youtube.com "no hagas clic")

Output:

[![YouTube](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSWhfZCLVtXGkawxt6C2XjU4pAFQbQEOCc3cw&usqp=CAU)](https://www.youtube.com "no hagas clic")

<br>

## Crear tabla de contenidos:

```
- [Capítulo 1](#capitulo-1)

- [Capítulo 2](#capitulo-2)

- [Capítulo 3](#capitulo-3)

- [Capítulo 4](#capitulo-4)
```

Output:

- [Capítulo 1](#capitulo-1)

- [Capítulo 2](#capitulo-2)

- [Capítulo 3](#capitulo-3)

- [Capítulo 4](#capitulo-4)

---

_Link para ver mas sobre markdown:_
[https://www.markdown.org](https://www.markdownguide.org/)

_Guía en español de Joe D Castro:_
[https://joedicastro.com/pages/markdown.html](https://joedicastro.com/pages/markdown.html)

_Editor en línea de markdown:_
[https://www.dillinger.io](https://dillinger.io)

---

### Capitulo 1

### Capitulo 2

### Capitulo 3

### Capitulo 4
