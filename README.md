# 🚀 Portafolio de Proyectos & Showcases Técnicos — Álvaro

¡Bienvenido a mi repositorio de presentación de ingeniería de software! Aquí organizo y documento la arquitectura, stack tecnológico y características principales de mis mejores desarrollos.

> 🔒 **Monorepo de Showcases:** Para proteger los derechos de propiedad intelectual, credenciales y secretos de producción, el código fuente original de cada aplicación reside en un **repositorio privado**. En cada una de las carpetas de este showcase encontrarás la documentación técnica completa, diagramas de flujo en Mermaid y desglose del stack. Si eres un reclutador o líder técnico y deseas ver una **demo guiada por pantalla compartida**, estaré encantado de mostrártelo.

---

## 📂 Índice de Proyectos Destacados

### 1. 🎓 Aprender App — Simulador de Tests & Audio Podcast para Oposiciones
> Plataforma interactiva de estudio enfocada en oposiciones TIC del Estado (C1, A2, A1) con simulador de test por niveles, corrección dinámicas por tramos, modo audiolibro con voz sintetizada nativa y copia de seguridad en Google Drive.
* **Stack:** `React 19` | `Vite` | `Capacitor 8` | `FastAPI (Python)` | `Google Drive API` | `TTS Android Engine`
* 👉 **[Ver Detalles e Ingeniería de Aprender App](./aprender-app/README.md)**

---

### 2. 🤖 Agente Automático de InfoJobs — Bot RPA Autónomo
> Bot inteligente de automatización de empleo en Python con Playwright/Selenium. Analiza el CV en PDF, rastrea automáticamente ofertas de trabajo en InfoJobs según filtros de localización/tecnología y se inscribe sin intervención humana.
* **Stack:** `Python 3.10+` | `Playwright` | `Selenium` | `PyPDF2` | `JSON State Storage`
* 👉 **[Ver Detalles e Ingeniería del Agente InfoJobs](./buscar-trabajo/README.md)**

---

### 3. ⚡ High-Speed Android Transfer — Transferencia PC a Móvil (Rust + Kotlin)
> Sistema de transferencia de archivos ultrarrápido que reemplaza el lento protocolo MTP de Windows. Conecta un cliente de PC escrito en Rust Tokio con un servicio en Kotlin en Android mediante un flujo TCP directo (por USB ADB o Wi-Fi 6).
* **Stack:** `Rust 2021` | `Tokio Async` | `Kotlin (Android)` | `Coroutines` | `Direct ByteBuffers` | `Scoped Storage`
* 👉 **[Ver Detalles e Ingeniería de High-Speed Transfer](./high-speed-android-transfer/README.md)**

---

### 4. 🎬 Edit-Video — Editor Inteligente de Vídeo & Creador de Shorts
> Aplicación de escritorio desarrollada en Electron y React con motor interno en Python. Procesa el audio con FFmpeg para eliminar silencios, filtrar muletillas y extraer automáticamente los mejores momentos (*highlights*) recortándolos a formato vertical (Shorts/TikToks).
* **Stack:** `Electron` | `React 18` | `FastAPI (Python)` | `FFmpeg` | `MoviePy` | `Tailwind CSS`
* 👉 **[Ver Detalles e Ingeniería de Edit-Video](./edit-video/README.md)**

---

### 5. 🔍 LikeTurnitin — Calibrador de Detección de Plagio e IA
> Motor de análisis lingüístico avanzado diseñado para evaluar textos académicos en español. Mide perplejidad y *burstiness* estructural para calcular el porcentaje de autoría por IA y similitud con un 41% de paridad calibrada.
* **Stack:** `Python 3.10+` | `NLP Heuristics` | `PyTorch / Transformers` | `pdfplumber` | `ReportLab`
* 👉 **[Ver Detalles e Ingeniería de LikeTurnitin](./liketurnitin/README.md)**

---

### 6. 📱 Convertidor HTML a APK — App Nativa de Test Oposiciones TIC (Offline)
> Empaquetado nativo para Android mediante Capacitor de una plataforma de exámenes TIC con más de 100 test cargados localmente en JSON, funcionamiento 100% sin conexión y lectura de preguntas por voz nativa.
* **Stack:** `Capacitor 8` | `Android SDK` | `JavaScript ES6+` | `Vite` | `Gradle`
* 👉 **[Ver Detalles de Convertidor HTML a APK](./convertidor-html-apk/README.md)**

---

### 7. 💅 App de Reservas Comercial — Plataforma Web de Citas & Panel Admin
> Aplicación web comercial desplegada para un salón de estética. Incluye un portal mobile-first de reservas para clientes y un panel de administración privado donde la propietaria gestiona citas, servicios y horarios en tiempo real.
* **Stack:** `FastAPI` | `Python` | `SQLite` | `SQLAlchemy` | `JavaScript Mobile-First`
* 👉 **[Ver Detalles de la App de Reservas](./reserva-manicura/README.md)**

---

### 8. 🎮 Tower of Elements & JuegosRaiz — Juegos 3D WebGL e IA Multi-Agente (MARL)
> Proyecto de videojuegos 3D en el navegador usando Three.js y React Three Fiber con materiales Toon Shading personalizados, junto a simulaciones de IA en Python con PyTorch donde múltiples bots aprenden a jugar al fútbol con Aprendizaje por Refuerzo.
* **Stack:** `Three.js` | `React Three Fiber` | `TypeScript` | `PyTorch` | `Gymnasium / PettingZoo`
* 👉 **[Ver Detalles de Tower of Elements & JuegosRaiz](./tower-of-elements/README.md)**

---

### 9. 🧩 DevLens / Console Log Ninja — Extensión de Depuración Visual para VS Code
> Extensión desarrollada para Visual Studio Code que acelera el flujo de depuración en TypeScript y JavaScript insertando y limpiando logs contextuales de forma automatizada mediante análisis del árbol de sintaxis abstracta (AST).
* **Stack:** `VS Code Extension API` | `TypeScript` | `Node.js`
* 👉 **[Ver Detalles de DevLens / Console Log Ninja](./devlens-vscode/README.md)**

---

## 🛠️ Resumen Global del Stack de Ingeniería

* **Frontend:** React (v18/v19), Vite, TypeScript, Tailwind CSS, Electron, Three.js / React Three Fiber, HTML5/CSS3.
* **Backend & Sistemas:** Python (FastAPI, Uvicorn), Rust (Tokio async), Node.js, SQLite, SQLAlchemy.
* **Automatización & IA:** Playwright, Selenium, PyTorch, Transformers, NLP (Perplexiy & Burstiness), Scraping (BeautifulSoup), MARL.
* **Móvil & Protocolos:** Capacitor 8 (Android SDK), Kotlin Coroutines, Sockets TCP directos, Android Scoped Storage, TTS Native Plugins.

---

## 📬 Contacto & Videollamada Técnica

Si deseas revisar el código fuente completo o ver cualquiera de estos proyectos en ejecución a través de una demo técnica por pantalla compartida:

* **GitHub:** [alvaro-fullstack](https://github.com/)
* **Email:** *Disponible en mi CV / Perfil*
