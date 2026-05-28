# Convertidor y Optimizador Universal de Imágenes (CONV2JPG)

[![Licencia: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
![Vanilla JS](https://img.shields.io/badge/Vanilla-JS-yellow)
[![Privacidad](https://img.shields.io/badge/privacy-100%25%20Local-orange)](https://developer.mozilla.org/en-US/docs/Web/Privacy)

Una herramienta web ligera, moderna y **100% offline** diseñada para procesar, optimizar y renombrar lotes de imágenes de forma masiva sin comprometer tu privacidad. Todo el procesamiento ocurre localmente en el navegador, sin subir archivos a ningún servidor.

---

![Captura de pantalla de TextMetrika](screenshots/imagen2.png)

---

## ✨ Características Principales

* **Compatibilidad Universal:** Soporta la carga y procesamiento de múltiples formatos de imagen (PNG, JPG, WebP, GIF, etc.).
* **Compresión y Optimización:** Ajuste de la calidad de salida en formato JPEG y selección personalizada del color de fondo para transparencias.
* **Redimensionado Inteligente:** Escala el ancho de las imágenes de forma proporcional manteniendo una alta fidelidad y nitidez mediante algoritmos de suavizado avanzado (`imageSmoothingQuality: 'high'`).
* **Extractor de Metadatos PNG:** Si el archivo de origen es un PNG y contiene metadatos embebidos (chunks `tEXt`/`iTXt`), genera automáticamente un archivo `.txt` descriptivo asociado.
* **Renombrado por Lotes:** Permite definir un prefijo y una numeración secuencial automática para organizar tus archivos cómodamente.
* **Modo Oscuro Integrado:** Interfaz adaptativa visualmente cómoda mediante variables CSS nativas (conmutador 🌙/☀️).
* **Soporte Bilingüe:** Arquitectura internacionalizada con cambio dinámico e instantáneo entre Español e Inglés (ES/EN).

---

## 💾 Sistemas de Guardado Inteligente (Híbrido)

La aplicación detecta automáticamente las capacidades de tu navegador actual para ofrecerte la mejor experiencia de usuario:

1. **Modo Directo a Carpeta (Navegadores Chromium - Chrome, Edge, Opera, Brave):** Utiliza la *File System Access API*. Te permite seleccionar una carpeta local de tu ordenador y guarda en ella de forma directa todo el lote de imágenes y archivos de texto procesados con un solo clic.
2. **Modo Fallback Unificado a ZIP (Firefox, Safari, etc.):** Dado que estos navegadores restringen el acceso directo a carpetas por privacidad, la aplicación empaqueta automáticamente todo el lote procesado en un único archivo comprimido `.zip` de forma local usando la librería `JSZip`, evitando así la molesta apertura de decenas de ventanas de descarga individuales.
3. **Descarga Individual:** Permite descargar los archivos procesados uno a uno si solo necesitas gestionar pocas imágenes.

---

## 🚀 Cómo Utilizar

Al estar diseñada con tecnologías web nativas, no requiere de servidores, bases de datos ni complejas instalaciones de Node.js/npm.

1. Clona o descarga este repositorio en tu equipo.
2. Asegúrate de mantener juntos en el mismo directorio los archivos `index.html` y `jszip.min.js`.
3. Doble clic sobre `index.html` para abrirlo en cualquier navegador moderno.
4. ¡Listo! Puedes trabajar de manera **100% offline** (incluso sin conexión a internet).

📂 tu-carpeta-del-proyecto/
├── 📄 index.html   <-- Archivo principal de la aplicación
└── 📄 jszip.min.js       <-- Librería local para soporte ZIP offline

---

## 🛠️ Tecnologías Utilizadas

* **HTML5** (Estructura semántica)
* **CSS3** (Variables nativas, diseño fluido y transiciones de estado)
* **Vanilla JavaScript** (Manipulación del DOM, Canvas 2D API, DataView para lectura binaria de chunks y File System Access API)
* **JSZip.js** (Compresión local para entornos restringidos)

---

## 📝 Próximas Mejoras (To-Do)

- [x] Depurar y modernizar el estilo estético del CSS.
- [x] Añadir soporte bilingüe (Español/Inglés).
- [x] Implementar el conmutador de Modo Oscuro nativo.
- [ ] Implementar un área de *Drag & Drop* (arrastrar y soltar) para agilizar la carga de imágenes.
- [ ] Permitir la exportación masiva a formatos alternativos (ej. WebP).