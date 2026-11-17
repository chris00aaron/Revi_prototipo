# RÉVI — Jewelry Collection

Prototipo estático de una tienda visual. Abre `index.html` en el navegador; no requiere instalación ni compilación. La tipografía de Google Fonts requiere conexión a internet; se muestran alternativas locales si no hay conexión.

## Personalización

- **Nueva paleta:** agrega un bloque `html[data-theme="id"]` en `styles.css` definiendo `--bg`, `--surface`, `--text`, `--text-muted`, `--gold`, `--accent`, `--accent-hover`, `--accent-contrast` y `--border`. Añade su nombre y muestras al arreglo `themes` en `app.js`. Comprueba el contraste de texto y botones con WCAG AA.
- **Fotos reales:** reemplaza las ilustraciones CSS de `.product-image`, `.hero-art` y `.social-tile` en `styles.css` / `index.html` por `<img>` con texto `alt` descriptivo. Para productos, el marcado lo genera `productCard()` en `app.js`; coloca allí la imagen y añade a los datos la ruta de foto que necesites.
- **Pasarela:** el botón `Finalizar compra` llama a `notice.showModal()` en `app.js`. Ahí se conectaría el flujo de checkout del proveedor cuando se defina la integración; ahora solo muestra una maqueta informativa.

Los productos de ejemplo y sus campos están en `products.js`.
