# Web del libro - Ingeniería del software seguro en la era de la IA generativa

Sitio estático (una sola página) para presentar el libro y sus diapositivas, pensado para publicarse
con **GitHub Pages**.

## Contenido

```
web-libro-ia-generativa/
├── index.html          Página principal (portada, descripción, diapositivas, cómo citar)
├── styles.css          Hoja de estilos
├── .nojekyll           Evita el procesado Jekyll de GitHub Pages
├── img/
│   ├── ule.png         Logotipo de la Universidad de León (cabecera)
│   ├── book_cover.png  Portada del libro (miniatura enlazada al PDF)
│   └── slides/         Miniaturas (primera diapositiva) de cada capítulo/anexo
└── pdf/
    ├── libro.pdf       Libro completo (v1.3, 287 páginas)
    └── slides/         Diapositivas por capítulo/anexo (versión alumnado)
```

## Publicación en GitHub Pages

1. Crea un repositorio nuevo (por ejemplo `web_libro_ia_generativa_segura`).
2. Sube el contenido de esta carpeta a la raíz del repositorio.
3. En *Settings → Pages*, selecciona la rama `main` y la carpeta `/ (root)`.
4. La web quedará disponible en `https://<usuario>.github.io/<repositorio>/`.

El archivo `.nojekyll` garantiza que los ficheros se sirvan tal cual.

## Actualizar el contenido

- **Libro:** sustituye `pdf/libro.pdf` por la nueva compilación.
- **Diapositivas:** sustituye los PDF de `pdf/slides/` y regenera las miniaturas en `img/slides/`
  (primera página de cada mazo, en PNG).
- **Portada:** sustituye `img/book_cover.png` por la nueva portada renderizada.

## Licencia

El contenido del libro se distribuye bajo **CC BY-NC-ND 4.0**.
