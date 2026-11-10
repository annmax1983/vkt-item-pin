# VKT Item Pin

[English](../README.md) | [中文](README_zh.md) | Español | [Deutsch](README_de.md) | [日本語](README_ja.md) | [Français](README_fr.md)

Una extensión de navegador para investigar compras: captura instantáneas de productos con solo pasar el cursor. El título, el precio, el enlace, el modelo, el sitio y la fecha se guardan en una biblioteca local, con seguimiento automático del historial de precios.

> Chrome / Edge / Firefox · Manifest V3 · Permisos mínimos · Sin rastreo · 100 % local

---

## ¿Por qué VKT Item Pin?

Comparar productos entre tiendas suele significar decenas de pestañas abiertas y copiar y pegar en hojas de cálculo. VKT Item Pin te permite pasar el cursor sobre cualquier producto, hacer clic en **Pin** y construir una biblioteca con seguimiento de precios, directamente en tu navegador.

| Ventaja | Detalle |
|---------|---------|
| 🎯 **Captura al pasar el cursor** | Pasa el cursor y pulsa Pin: título, precio, enlace, modelo, sitio y fecha se extraen automáticamente |
| 🔁 **Precio registrado automáticamente** | Vuelve a abrir un producto que ya fijaste y el precio se registra solo, sin un segundo clic |
| 🔔 **Alerta de precio local (Pro)** | Define un precio objetivo por producto: la primera visita que lo alcance o baje de él muestra una notificación del sistema, sin servidor ni correo |
| 📈 **Historial de precios** | Cada captura, manual o automática, añade un punto y crea la gráfica de tendencia |
| 🛒 **24 sitios preconfigurados** | Selectores ajustados para Amazon, eBay, Etsy, Walmart, AliExpress, Temu y más, además de un motor universal (JSON-LD / OG / selectores genéricos) para cualquier otra tienda |
| 🏷 **Notas y etiquetas** | Anota el motivo («esperar al Black Friday») y organiza con hasta 10 etiquetas por producto, todo buscable |
| 🖼️ **Miniaturas** | Cada registro guarda la imagen del producto |
| 🔒 **Privacidad primero** | Todos los datos permanecen en tu navegador con `storage.local`. No se sube nada |

---

## Funciones

### 🆓 Gratis

| Función | Descripción |
|---------|-------------|
| 🎯 **Captura con un clic** | Fija cualquier producto en páginas de detalle o listados de búsqueda |
| 📋 **Vista previa y selección** | Edita los campos antes de guardar; el modo «Elegir» permite hacer clic en cualquier elemento para rellenar un campo |
| 🔁 **Historial automático** | Al abrir de nuevo un producto fijado, el precio se registra en segundo plano: un punto por día como máximo |
| 📈 **Historial de precios** | Recapturas ilimitadas en productos seguidos, con gráfica de tendencia por producto |
| 🏷 **Notas y etiquetas** | Una nota libre y hasta 10 etiquetas por producto; se pueden buscar, filtrar y exportar |
| 🔍 **Filtros y orden** | Filtra por sitio o etiqueta y ordena por última actividad, mayor bajada o precio |
| 📊 **Estadísticas** | Franja resumen: cuántos productos bajaron en 30 días |
| 🧭 **Comparar fuera** | Un clic para buscar el mismo título en Google Shopping, eBay o Amazon |
| ✏️ **Editar registros** | Corrige títulos y modelos, corrige o elimina puntos de precio erróneos, cambia notas y etiquetas (el precio objetivo es Pro) |
| 💾 **Copia JSON** | Exporta / importa una copia completa de tu biblioteca (sin conexión), incluidas notas, etiquetas y precios objetivo |
| 📤 **Exportar CSV** | Formato largo (una fila por punto de precio, con BOM, compatible con Excel) incluyendo notas, etiquetas y precio objetivo |
| 🧮 **Monitor de almacenamiento** | Muestra el uso real y avisa antes de llenarse |
| 🌍 **6 idiomas** | Inglés, chino, japonés, español, alemán, francés |

### ⭐ Pro (requiere licencia)

| Función | Descripción |
|---------|-------------|
| 🔔 **Alerta de precio objetivo** | Define un precio objetivo por producto; la primera visita que lo alcanza lanza una notificación del sistema (todo local, con interruptor en el panel) |
| ♾️ **Productos ilimitados** | El plan gratuito cubre 10 productos; Pro elimina el límite (las recapturas nunca cuentan) |
| 🔍 **Filtros avanzados** | Filtra por rango de fechas y rango de precios (los filtros por sitio y etiqueta son gratuitos) |
| 📊 **Comparar productos** | Superpone el historial de precios de hasta 6 productos en una sola gráfica |

---

## Sitios compatibles

**Preajustes manuales (24):** Amazon (todos los mercados), eBay, Etsy, Walmart, Target, AliExpress, Temu, Best Buy, Home Depot, Lowe's, Newegg, Wayfair, Mercari, Shopee, Lazada, Rakuten, SHEIN, Alibaba.com / 1688, DHgate, TikTok Shop, bol.com, Allegro, Otto.de, Cdiscount…

**Todo lo demás** (Shopify / WooCommerce / tiendas independientes) queda cubierto por el motor universal: datos estructurados JSON-LD → etiquetas Open Graph → selectores genéricos → expresiones regulares → modo de selección manual.

---

## Navegadores compatibles

| Navegador | Estado |
|---------|--------|
| Google Chrome | ✅ Totalmente compatible |
| Microsoft Edge | ✅ Totalmente compatible |
| Mozilla Firefox | ✅ Totalmente compatible |
| Otros navegadores basados en Chromium | ✅ Debería funcionar |

> **Nota sobre Firefox:** la captura al pasar el cursor, la vista previa, el seguimiento automático de precios, las alertas de precio objetivo, el historial de precios, las notas y etiquetas, la biblioteca y la copia JSON se comportan igual en los tres navegadores. Chrome, Edge y Firefox usan la misma interfaz de **ventana emergente de la barra de herramientas**; la única diferencia es la implementación en segundo plano (service worker en Chromium, página de eventos en Firefox). Firefox solicita `activeTab`, `scripting`, `storage`, `notifications`, `<all_urls>` y `https://api.annmax1983.com/*` (validación opcional de licencia Pro): el mismo conjunto que Chrome y Edge.

---

## Instalación

| Tienda | Enlace |
|---|---|
| Chrome Web Store | [Instalar en Chrome](https://chromewebstore.google.com/detail/ijimihnecmjmgllhibaljdocbkhfmjca) |
| Complementos de Microsoft Edge | [Instalar en Edge](https://microsoftedge.microsoft.com/addons/detail/ahgadlbdecpnpbjiajmaepekmehccpgh) |
| Complementos de Firefox (AMO) | [Instalar para Firefox](https://addons.mozilla.org/firefox/addon/vkt-item-pin/) |

> Instale solo desde las tiendas oficiales de arriba; evite sitios de descarga de terceros.

---

## Uso

### Capturar un producto

1. Pasa el cursor sobre un producto (en la página de detalle o en la cuadrícula de resultados) — aparecerá el botón 📌
2. Haz clic: se abre un panel lateral con el título, precio, enlace, modelo, sitio y fecha extraídos
3. Corrige lo que necesites, usa **Elegir** para completar un campo y pulsa **Guardar**

### Seguir precios

- Abre de nuevo un producto ya guardado: el precio se registra solo, un punto por día como máximo (el plan gratuito permite guardar hasta 10 productos; volver a registrar el precio de un producto ya guardado no añade un registro ni consume otra plaza)
- Define un **precio objetivo** en el panel: cuando una visita lleve el precio a ese valor o por debajo, verás una notificación del sistema, una sola vez por cruce y sin repetirse
- Abre el panel para ver la gráfica de tendencia, el resumen de bajadas de 30 días, o usa **Comparar** (Pro) para superponer varios productos
- Usa **nota** y **etiquetas** para recordar por qué merece la pena esperar

### Copia de seguridad

- El pie del panel incluye **Copia JSON** / **Importar** — recomendado periódicamente, ya que los datos solo viven en tu navegador

---

## Privacidad

- `storage` — Guarda tu biblioteca localmente. Ningún contenido de página sale de tu navegador.
- `scripting` + `activeTab` — Inyectan el botón Pin / extraen campos solo mientras interactúas con la página.
- `notifications` — Solo se usa para las alertas locales de precio objetivo (Pro); no se envía nada a ningún sitio.
- `<all_urls>` — Permite funcionar en cualquier tienda. Nunca lee ni sube contenido en segundo plano.
- Sin rastreo ni analíticas. Las solicitudes de red se limitan a la activación/validación de la licencia Pro y a las miniaturas de productos, que se cargan directamente desde el sitio original.

---

## Aviso sobre el código fuente

> ⚠️ **Este repositorio es solo para presentar el proyecto: el código fuente completo no se publica aquí.** Solo contiene la documentación de uso, las notas de versión y la información de soporte de la extensión.

> 📥 **Descárgala e instálala únicamente desde las tiendas oficiales de navegadores:** Chrome Web Store · Microsoft Edge Add-ons · Complementos de Firefox (AMO). Desde aquí no se distribuye ningún instalador sin conexión.

---

## Licencia

Copyright © 2026 VKT Item Pin. Todos los derechos reservados.

Este software es propietario y de código cerrado. Sin autorización previa por escrito del autor, queda estrictamente prohibido descompilar, aplicar ingeniería inversa, crackear, modificar, reempaquetar, redistribuir o revender el programa (total o parcialmente).

---

## ❤️ Apoya el proyecto

Si VKT Item Pin te resulta útil, ¡considera apoyar el proyecto!

**[👉 Obtener clave de licencia](https://annmax1983.com/checkout?plugin=itempin)** · [GitHub](https://github.com/annmax1983/ItemPin) · [Sitio oficial](https://www.annmax1983.com/extensions/itempin)

---

## Enlaces

- **☕ Apoya el proyecto (Ko-fi):** https://ko-fi.com/annmax?ref=vkt-item-pin
