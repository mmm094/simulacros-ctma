# Simulacros CTMA · Primer parcial

Web de simulacros tipo test de Ciencia y Tecnología del Medio Ambiente.
Desarrollado por **Miguel Martos**.

## Publicarla en GitHub Pages
1. Crea un repositorio nuevo en GitHub (por ejemplo `simulacros-ctma`), público.
2. Pulsa **Add file → Upload files** y sube `index.html` (y este `README.md`).
3. Ve a **Settings → Pages**. En *Source* elige **Deploy from a branch**, rama **main**, carpeta **/(root)** y pulsa **Save**.
4. En 1-2 minutos la web estará en `https://TU-USUARIO.github.io/simulacros-ctma/`.

## Añadir preguntas nuevas
Abre `index.html`, busca `const BANK = [` y añade cada pregunta **al final de la lista** con este formato:

```js
["T3","Texto de la pregunta",["Opción correcta","Opción 2","Opción 3","Opción 4"],0,"Explicación breve"],
```

- El primer campo es el tema: T1, T2a, T2b, T3, T4, T5 (teoría) o P1, P2, P3 (prácticas).
- El número es la posición de la opción correcta (0 = la primera). Las opciones se mezclan solas.
- Para preguntas tipo "A y B son verdaderas", añade `,1` al final para que no se mezclen las opciones.
- Para una práctica nueva (por ejemplo la 4), añade `P4: "Práctica 4: ..."` dentro de `TEMAS`.
