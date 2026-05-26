# 📸 Convertidor y Redimensionador de Imágenes

¡Una utilidad web ultra-ligera, rápida y privada para procesar tus fotografías e imágenes directamente desde tu navegador! Sin servidores, sin rastreadores y sin necesidad de conexión a internet.

[![Licencia: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![JavaScript](https://img.shields.io/badge/JavaScript-Pure-F7DF1E?logo=javascript&logoColor=black)](https://developer.mozilla.org/es/docs/Web/JavaScript)
[![HTML5](https://img.shields.io/badge/HTML5-Pure-E34F26?logo=html5&logoColor=white)](https://developer.mozilla.org/es/docs/Web/HTML)
[![CSS3](https://img.shields.io/badge/CSS3-Pure-1572B6?logo=css3&logoColor=white)](https://developer.mozilla.org/es/docs/Web/CSS)

---

## 🚀 Funcionalidades Principales

- **🔄 Conversión de Formatos:** Cambia el formato de tus imágenes al vuelo (soporta JPEG, PNG y más).
- **📐 Escalado Bidireccional Inteligente:** Redimensiona tus imágenes tanto para reducirlas como para ampliarlas manteniendo siempre la proporción original y con algoritmos de suavizado para máxima nitidez.
- **🌓 Modo Oscuro Integrado:** Interfaz adaptable con un solo clic para descansar la vista.
- **🌐 Soporte Bilingüe:** Cambia instantáneamente entre **Español** e **Inglés** sin necesidad de refrescar la página.
- **🔒 Privacidad 100% Garantizada:** El procesamiento se realiza de forma local mediante el API de Canvas de JavaScript. Tus imágenes nunca se suben a ningún servidor.

---

## 💻 Vista previa de la Aplicación

![Imagen mostrando aplicación 1](/screenshots/imagen.png)

---

## 🛠️ Cómo Utilizar

**`index.html`** es el único archivo necesario para que todo funcione. Al ser una aplicación portátil (Serverless), se puede ejecutar desde cualquier ubicación:
* 💾 Disco duro local.
* 🔌 Memoria USB o disco externo.
* 🌐 Desplegado en GitHub Pages, Vercel, Netlify, etc.

### Pasos:
1. Haz doble clic en el archivo `index.html` para abrirlo en tu navegador favorito.
2. Selecciona la imagen que deseas modificar.
3. Elige el formato de destino y define el nuevo tamaño máximo (ancho o alto en píxeles). *Nota: Dejar estos campos vacíos mantendrá el tamaño original.*
4. Haz clic en **Procesar Imagen** para generar la vista previa.
5. Haz clic en el botón de **Descargar** ¡y listo!

---

## 🏗️ Stack Tecnológico

Este proyecto fue desarrollado bajo la filosofía *Vanilla Web*, garantizando que sea extremadamente rápido y no requiera de pesadas dependencias ni librerías adicionales:
- **HTML5:** Estructura semántica.
- **CSS3:** Diseño responsivo basado en Variables CSS nativas para el intercambio de temas.
- **JavaScript (Vanilla):** Lógica de traducción, manejo del DOM dinámico y API de `HTML5 Canvas` para el renderizado y compresión de imágenes.

---

## 📌 Historial de Actualizaciones (Mayo 2026)

- [x] **Tema Dinámico:** Añadida opción nativa para activar el Modo Oscuro.
- [x] **Internacionalización (i18n):** Implementado selector de idioma (Español / Inglés) con persistencia en `localStorage`.
- [x] **Algoritmo de Escalado:** Motor de redimensión optimizado con interpolación de alta calidad (`imageSmoothingQuality`) para evitar imágenes pixeladas al ampliarlas.

---

## 🔮 Próximos Pasos (To-Do)

¿Tienes alguna idea para mejorar esta herramienta? ¡Las sugerencias y contribuciones son más que bienvenidas! Sientete libre de abrir un *Issue* o enviar un *Pull Request*.

Algunas ideas en el radar:
- [ ] Soporte para procesamiento por lotes (múltiples imágenes a la vez).
- [ ] Función de arrastrar y soltar (*Drag and Drop*) para cargar archivos.
- [ ] Soporte de conversión para nuevos formatos como WebP.

---
Desarrollado con ❤️ por [Einsam70](https://github.com/Einsam70)