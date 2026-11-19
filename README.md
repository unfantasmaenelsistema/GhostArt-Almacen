<div align="center">
  <img src="assets/logo.png" alt="Un Fantasma en el Sistema" width="90">

# GhostArt Almacén

Almacén de imágenes y GIF de [GhostArt](https://github.com/unfantasmaenelsistema/GhostArt).

▶ **Se ven en la galería:** https://unfantasmaenelsistema.github.io/GhostArt/

</div>

## Para qué sirve

La galería principal publica todo su contenido en GitHub Pages, que tiene un tope de unos 1 GB por sitio.
Para no toparse con él, las imágenes nuevas viven aquí y **la galería principal las muestra como si fueran suyas**
(lee el `manifest.json` de este repo cada pocas horas y en cada despliegue).

## Cómo añadir contenido

- Imágenes: `img/<categoría>/nombre.webp` (cualquier formato; la Action lo convierte a WebP).
- GIF: `gifs/nombre.gif` (se conservan tal cual; la miniatura es el primer fotograma).
- Cada push regenera `manifest.json` y las miniaturas con [`tools/ghostart.py`](tools/ghostart.py).
- Para que aparezca ya en la galería, lanza *Actions → Galería (procesar y publicar) → Run workflow* en GhostArt;
  si no, entra sola en la siguiente pasada (cada 6 h).

## Cuándo abrir otro almacén

Cuando éste se acerque a ~800 MB: crea `GhostArt-Almacen-2` igual que éste, activa Pages (Source: GitHub Actions) y
añádelo a [`almacenes.json`](https://github.com/unfantasmaenelsistema/GhostArt/blob/main/almacenes.json) de GhostArt.

## Licencia

Imágenes: [CC BY 4.0](LICENSE-IMAGES.md). Código: [MIT](LICENSE).
