# 1DAM Interactivo

Recursos interactivos (HTML autocontenidos) de apoyo a los apuntes de
[🤖 1ºDAM Programación](https://martinezpenya.es/1DAMProgramacion/).

Publicado con GitHub Pages en <https://martinezpenya.es/1DAMInteractivo/>.

## Recursos

| Unidad | Recurso | Descripción |
|---|---|---|
| UD04 · Recursividad | [`recursividad/`](https://martinezpenya.es/1DAMInteractivo/recursividad/) | Recursividad paso a paso con `factorial(n)` y `fibonacci(n)`: pila de llamadas (stack), ocupación de memoria, árbol de llamadas (Fibonacci), desbordamiento aritmético (`int`/`long`) y `StackOverflowError`. |

### Enlazar un caso concreto

`recursividad/` acepta parámetros opcionales en la URL:

| Parámetro | Valores | Por defecto |
|---|---|---|
| `alg` | `factorial` o `fibonacci` | `factorial` |
| `n` | 0–100 (factorial), 0–8 (fibonacci) | 4 (factorial), 5 (fibonacci) |
| `tipo` | `int` o `long` (solo factorial) | `int` |
| `pila` | 3–60 (tamaño de la pila en marcos) | 25 |
| `paso` | número de paso (empieza en 1) | 1 |

Ejemplos: `recursividad/?n=13&tipo=int` muestra el desbordamiento de `int`; `recursividad/?alg=fibonacci&n=5`, el árbol de llamadas de `fibonacci(5)`.

## Incrustar un recurso en los apuntes

```html
<iframe src="https://martinezpenya.es/1DAMInteractivo/recursividad/"
        width="100%" height="900" loading="lazy" frameborder="0"></iframe>
```

En los apuntes (MkDocs) se envuelve en `<div class="solo-web" markdown>` para que no salga en el PDF.

## Normas para añadir recursos

- **Cada página HTML debe incluir el banner de origen** (bloque `<div class="origen">` y sus estilos,
  marcados con el comentario «Banner de origen»). Enlaza a los apuntes para que, si alguien incrusta
  el recurso en otra web, se vea de dónde procede. Cópialo tal cual de `index.html`.
- Un recurso = un HTML autocontenido (CSS y JS en línea, sin dependencias salvo Google Fonts), dentro
  de una carpeta por tema (`recursividad/`, `arrays/`, …).
- Textos en español de España. Tema claro y oscuro, y que funcione a ancho de móvil y dentro de un iframe.
- Añade el recurso a la tabla de este README y a la lista de `index.html`.

## Licencia

[1DAM Interactivo](https://martinezpenya.es/1DAMInteractivo/) © 2026 by [David Martínez](https://github.com/martinezpenya)
is licensed under [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/).
