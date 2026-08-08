# 🤖 Agente Autónomo de Búsqueda de Empleo — Auto-Apply para InfoJobs

[![Python](https://img.shields.io/badge/Python-3.10+-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)
[![Playwright](https://img.shields.io/badge/Playwright-Automation-45BA4B?style=for-the-badge&logo=playwright&logoColor=white)](https://playwright.dev/)
[![Selenium](https://img.shields.io/badge/Selenium-Browser-43B02A?style=for-the-badge&logo=selenium&logoColor=white)](https://www.selenium.dev/)
[![JSON](https://img.shields.io/badge/Data-JSON_Storage-000000?style=for-the-badge&logo=json&logoColor=white)]()

**Agente Autónomo de Búsqueda de Empleo** es una solución de ingeniería de automatización RPA (Robotic Process Automation) diseñada para realizar búsquedas activas de empleo, análisis de perfil y postulación automática en plataformas como InfoJobs sin intervención humana.

> 🔒 **Nota sobre el código fuente:** Este es un repositorio público de presentación (*Showcase*). Las credenciales de acceso, cookies de sesión, datos personales del CV y scripts con selectores privados se omiten en este repositorio por seguridad. Para una demostración en vivo de la automatización en ejecución, contáctame para una demo por pantalla compartida.

---

## 💡 ¿Qué problema resuelve?

Buscar trabajo manualmente requiere horas diarias de tareas repetitivas: buscar ofertas, filtrar por zona/tecnología, abrir formularios de solicitud, adjuntar currículums y responder preguntas habituales de los reclutadores.

Este bot inteligente **automatiza el 100% del proceso**:
* Lee el perfil del candidato desde su CV en formato PDF.
* Rastrea InfoJobs por palabras clave, categorías técnicas y ubicaciones geográficas.
* Analiza las ofertas y realiza el proceso completo de inscripción (*Auto-Apply*).
* Guarda un registro estructurado para evitar duplicados.

---

## 🎯 Características Principales

### 1. 🔍 Navegación y Extracción Automatizada
* **Búsqueda Avanzada:** Rastreos por palabras clave (*React, Python, Full Stack, DevOps*), filtrando por modalidad (Remoto, Híbrido, Presencial) y ubicaciones.
* **Manejo de DOM Dinámico:** Estrategias avanzadas de selectores CSS y XPath que se adaptan a cambios menores en la interfaz de InfoJobs.

### 2. ⚡ Proceso de Inscripción Inteligente (Auto-Apply)
* **Gestión de Formularios:** Automatización del flujo de postulación, interactuando con botones de confirmación, menús desplegables y campos de texto.
* **Bypass de Bloqueos & Cookies:** Inyección de cookies de sesión autenticadas previamente y gestión de diálogos de consentimiento GDPR.

### 3. 📊 Control de Estado y Persistencia
* **Prevención de Duplicados:** Almacena los identificadores de ofertas procesadas en un archivo de estado local (`solicitudes.json`).
* **Logs en Tiempo Real:** Registro detallado de ofertas inspeccionadas, inscripciones completadas y errores de formulario.

---

## 🛠️ Arquitectura Técnica

```mermaid
graph TD
    A[Perfil & CV PDF del Candidato] --> B[Agente Autónomo de Python]
    B -->|Playwright / Selenium Engine| C[Navegador Headless / Chromium]
    C -->|Búsqueda y Filtrado| D[InfoJobs Platform]
    D -->|Extracción de Oferta| E{¿Encaja con Perfil?}
    E -->|Sí| F[Auto-Apply: Iniciar Sesión y Completar Formulario]
    E -->|No| G[Descartar Oferta]
    F -->|Éxito| H[Persistir Registro en solicitudes.json]
```

### 💻 Stack Tecnológico
* **Python 3.10+:** Lenguaje base para el control asíncrono y procesamiento.
* **Playwright & Selenium:** Automatización y renderizado completo del navegador para interactuar con aplicaciones de página única (SPA).
* **PyPDF2 / pdfplumber:** Análisis y extracción de texto de currículums en formato PDF.
* **JSON State Management:** Almacenamiento ligero de candidaturas y estados.
