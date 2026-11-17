# Créditos de las imágenes de producto

Las imágenes de `img/productos/` son fotografías oficiales de catálogo de cada marca,
recortadas y normalizadas para la tienda. Cada archivo final es un WebP de 900 × 900 px
con fondo transparente.

| Archivo | Producto en la tienda | Modelo real de la foto | Marca / origen |
| --- | --- | --- | --- |
| `tenis-runner-pro.webp` | Tenis Runner Pro (tallas 40 y 42) | Air Zoom Pegasus 41 (running) | [Nike](https://www.nike.com/) |
| `tenis-urban-classic.webp` | Tenis Urban Classic (talla 39) | Superstar (EG4959, negra con franjas blancas) | [Adidas](https://www.adidas.com/) |
| `mocasin-elegance.webp` | Mocasín Elegance (talla 41) | Benedict Loafer, cuero marrón | [Hush Puppies](https://www.hushpuppies.co.uk/) |
| `bota-trail-max.webp` | Bota Trail Max (talla 43) | Newton Ridge Plus II Waterproof, hiking | [Columbia](https://www.columbia.com/) |
| `sandalia-verano.webp` | Sandalia Verano (talla 38) | Arizona Suede Leather (1026200, verde) | [Birkenstock](https://www.birkenstock.com/) |
| `zapatillas-futbol.webp` | Zapatillas para fútbol (talla 40) | Predator Club FG/MG (ID1326, roja) | [Adidas](https://www.adidas.com/) |

## Tratamiento aplicado

1. Se partió de la foto de producto oficial (fondo blanco o gris de estudio).
2. Se eliminó el fondo con IA (`rembg`, modelo `isnet-general-use`).
3. Se recortó al producto, se centró y se ajustó a un lienzo cuadrado transparente de
   900 × 900 px con ~4,5 % de margen.
4. Se exportó a WebP con transparencia (calidad 92).

## Aviso de uso

Las fotografías y las marcas (Nike, Adidas, Hush Puppies, Columbia, Birkenstock) son
propiedad de sus titulares y se incluyen aquí con fines académicos/demostrativos para el proyecto
MIMO. Para publicar la tienda comercialmente debes sustituirlas por imágenes licenciadas
(prensa de marca, banco de imágenes propio o fotografía de producto contratada).

## Cómo cambiar una imagen

1. Guarda el archivo en `Frontend/img/productos/` (WebP o PNG con transparencia,
   idealmente 900 × 900 px).
2. En `admin-productos.html`, edita el producto y escribe la ruta relativa, por ejemplo
   `img/productos/mi-zapato.webp`. También se aceptan URLs `http/https`.
3. Actualiza esta tabla si la imagen viene de otra fuente.

Las imágenes se sirven localmente, así que el catálogo funciona incluso abriendo las
páginas con `file://`.
