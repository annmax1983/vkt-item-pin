# VKT Item Pin

[English](../README.md) | [中文](README_zh.md) | Español | [Deutsch](README_de.md) | [日本語](README_ja.md) | [Français](README_fr.md)

Una extensión de navegador para investigar compras: captura instantáneas de productos con solo pasar el cursor. El título, el precio, el enlace, el modelo, el sitio y la fecha se guardan en una biblioteca local, con seguimiento automático del historial de precios.

> Basado en Chromium · Manifest V3 · Permisos mínimos · Sin rastreo · 100 % local

---

## ¿Por qué VKT Item Pin?

Comparar productos entre tiendas suele significar decenas de pestañas abiertas y copiar y pegar en hojas de cálculo. VKT Item Pin te permite pasar el cursor sobre cualquier producto, hacer clic en **Pin** y construir una biblioteca con seguimiento de precios, directamente en tu navegador.

| Ventaja | Detalle |
|---------|---------|
| 🎯 **Captura al pasar el cursor** | Pasa el cursor y pulsa Pin: título, precio, enlace, modelo, sitio y fecha se extraen automáticamente |
| 📈 **Historial de precios** | Vuelve a capturar el mismo producto cuando quieras: cada visita añade un punto de precio y crea la gráfica de tendencia |
| 🛒 **24 sitios preconfigurados** | Selectores ajustados para Amazon, eBay, Etsy, Walmart, AliExpress, Temu y más, además de un motor universal (JSON-LD / OG / selectores genéricos) para cualquier otra tienda |
| 🖼️ **Miniaturas** | Cada registro guarda la imagen del producto |
| 🔒 **Privacidad primero** | Todos los datos permanecen en tu navegador con `chrome.storage.local`. No se sube nada |

---

## Funciones

### 🆓 Gratis

| Función | Descripción |
|---------|-------------|
| 🎯 **Captura con un clic** | Fija cualquier producto en páginas de detalle o listados de búsqueda |
| 📋 **Vista previa y selección** | Edita los campos antes de guardar; el modo «Elegir» permite hacer clic en cualquier elemento para rellenar un campo |
| 📈 **Historial de precios** | Recapturas ilimitadas en productos seguidos, con gráfica de tendencia por producto |
| ✏️ **Editar registros** | Corrige títulos y modelos, corrige o elimina puntos de precio erróneos |
| 💾 **Copia JSON** | Exporta / importa una copia completa de tu biblioteca (sin conexión) |
| 🧮 **Monitor de almacenamiento** | Muestra el uso real y avisa antes de llenarse |
| 🌍 **6 idiomas** | Inglés, chino, japonés, español, alemán, francés |

### ⭐ Pro (requiere licencia)

| Función | Descripción |
|---------|-------------|
| ♾️ **Productos ilimitados** | El plan gratuito cubre 50 productos; Pro elimina el límite |
| 🔍 **Filtros avanzados** | Filtra por sitio, rango de fechas y rango de precios |
| 📤 **Exportar CSV** | Exporta tu biblioteca (con BOM, compatible con Excel) |
| 📊 **Comparar productos** | Superpone el historial de precios de hasta 6 productos en una sola gráfica |

---

## Sitios compatibles

**Preajustes manuales (24):** Amazon (todos los mercados), eBay, Etsy, Walmart, Target, AliExpress, Temu, Best Buy, Home Depot, Lowe's, Newegg, Wayfair, Mercari, Shopee, Lazada, Rakuten, SHEIN, Alibaba.com / 1688, DHgate, TikTok Shop, bol.com, Allegro, Otto.de, Cdiscount…

**Todo lo demás** (Shopify / WooCommerce / tiendas independientes) queda cubierto por el motor universal: datos estructurados JSON-LD → etiquetas Open Graph → selectores genéricos → expresiones regulares → modo de selección manual.

---

## Instalación

1. Abre la página de extensiones: **Chrome** `chrome://extensions/` · **Edge** `edge://extensions/`
2. Activa el **Modo de desarrollador**
3. Pulsa **Cargar descomprimida** y selecciona la carpeta `vkt-item-pin`
4. Pasa el cursor sobre cualquier producto y pulsa el botón 📌 Pin

---

## Uso

### Capturar un producto

1. Pasa el cursor sobre un producto (en la página de detalle o en la cuadrícula de resultados) — aparecerá el botón 📌
2. Haz clic: se abre un panel lateral con el título, precio, enlace, modelo, sitio y fecha extraídos
3. Corrige lo que necesites, usa **Elegir** para completar un campo y pulsa **Guardar**

### Seguir precios

- Vuelve a capturar un producto guardado: se añade un punto de precio automáticamente (los productos seguidos nunca consumen el límite gratuito)
- Abre el panel para ver la gráfica de tendencia, o usa **Comparar** (Pro) para superponer varios productos

### Copia de seguridad

- El pie del panel incluye **Copia JSON** / **Importar** — recomendado periódicamente, ya que los datos solo viven en tu navegador

---

## Privacidad

- `storage` — Guarda tu biblioteca localmente. Ningún contenido de página sale de tu navegador.
- `scripting` + `activeTab` — Inyectan el botón Pin / extraen campos solo mientras interactúas con la página.
- `<all_urls>` — Permite funcionar en cualquier tienda. Nunca lee ni sube contenido en segundo plano.
- Sin rastreo ni analíticas. La única petición de red es la activación/validación de la licencia Pro.

---

## Licencia

Copyright © 2026 VKT Item Pin. Todos los derechos reservados.

---

## ❤️ Apoya el proyecto

Si VKT Item Pin te resulta útil, ¡considera apoyar el proyecto!

**[👉 Obtener clave de licencia](https://www.annmax1983.com/checkout.html?plugin=itempin)** · [GitHub](https://github.com/annmax1983/ItemPin) · [Sitio oficial](https://www.annmax1983.com/extensions/itempin)
