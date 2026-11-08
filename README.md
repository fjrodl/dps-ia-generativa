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

Sitio publicado automáticamente en:

**https://fjrodl.github.io/dps-ia-generativa/**

El despliegue lo ejecuta `.github/workflows/deploy.yml` en cada push a `main`
(flujo «Pages artifact» de GitHub Actions). No se recompila LaTeX: los PDFs
versionados en `pdf/` se publican tal cual.

Para habilitar Pages en un repositorio nuevo: *Settings → Pages → Source:
GitHub Actions* (o vía API con `build_type=workflow`). El archivo `.nojekyll`
garantiza que los ficheros se sirvan tal cual.

## Actualizar el contenido

- **Libro:** sustituye `pdf/libro.pdf` por la nueva compilación.
- **Diapositivas:** sustituye los PDF de `pdf/slides/` y regenera las miniaturas en `img/slides/`
  (primera página de cada mazo, en PNG).
- **Portada:** sustituye `img/book_cover.png` por la nueva portada renderizada.

## Licencia

El contenido del libro se distribuye bajo **CC BY-NC-ND 4.0**.
