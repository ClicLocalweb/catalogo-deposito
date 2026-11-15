# Portada del catálogo del depósito

Página de inicio del catálogo: un auto en el centro y, al hacer scroll, las líneas de productos salen volando desde el lugar del auto donde van. Cada pieza es un botón que lleva a su categoría.

Un solo archivo `index.html`, sin librerías.

## Cómo poner la foto del auto de verdad

1. Conseguí una foto de un auto de calle, **de costado y mirando a la derecha**, con fondo transparente o limpio (sirve Pexels o Unsplash, que son gratis).
2. Guardala como `auto.png` junto a `index.html`.

Listo. La página la usa sola; si el archivo no está, muestra el dibujo.

## Cómo poner las fotos de los productos

Guardá los archivos dentro de la carpeta `fotos/` con estos nombres:

| Archivo | Categoría |
|---|---|
| `fotos/filtros.webp` | Filtros |
| `fotos/aceite.webp` | Aceite de motor |
| `fotos/refrigerante.webp` | Refrigerante |
| `fotos/pastillas.webp` | Pastillas de freno |
| `fotos/escobillas.webp` | Escobillas |
| `fotos/aditivos.webp` | Aditivos para motor |
| `fotos/estetica.webp` | Estética vehicular |

Si una foto no está, se muestra el ícono dibujado. Conviene que sean cuadradas (por ejemplo 400×400) porque van dentro de un círculo.

## Cómo verla

Desde la carpeta:

```
python3 -m http.server 8000
```

y entrá a `http://localhost:8000`.

Para publicarla gratis con GitHub Pages: Settings, Pages, rama `main`, carpeta raíz.

## Pendiente

- Foto real del auto (reemplaza al dibujo).
- Fotos de los productos, con las imágenes de los proveedores.
- Que cada categoría lleve al listado real de productos.
