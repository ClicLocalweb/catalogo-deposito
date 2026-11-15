# Portada del catálogo del depósito

Página de inicio del catálogo: un auto en el centro y, al hacer scroll, las líneas de productos salen volando desde el lugar del auto donde van. Cada pieza es un botón que lleva a su categoría.

Un solo archivo `index.html`, sin librerías.

## Cómo funciona la escena

Son dos capas de la misma foto: `fondo.jpg` (la foto completa: ruta, guardarraíl, árboles) y `auto.png` (el auto recortado, sin fondo). Al bajar, el fondo se agranda despacio y el auto más rápido, y eso da la sensación de que la cámara se acerca. Cuando el auto queda en primer plano, el fondo se oscurece y salen las piezas.

En las dos capas la patente y el parabrisas están difuminados.

Para cambiar de foto hay que regenerar las dos capas y actualizar en `index.html` la línea `const AUTO = …` con la posición del auto dentro de la foto. Pedíselo a Claude con la foto nueva.

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
