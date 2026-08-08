# 💅 App de Reservas Comercial — Plataforma Web de Citas & Panel Admin

[![FastAPI](https://img.shields.io/badge/FastAPI-Python-009688?style=for-the-badge&logo=fastapi&logoColor=white)](https://fastapi.tiangolo.com/)
[![SQLite](https://img.shields.io/badge/SQLite-Database-003B57?style=for-the-badge&logo=sqlite&logoColor=white)](https://www.sqlite.org/)
[![JavaScript](https://img.shields.io/badge/JavaScript-Mobile_First-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)](https://developer.mozilla.org/)
[![HTML5/CSS3](https://img.shields.io/badge/HTML5_CSS3-Responsive-E34F26?style=for-the-badge&logo=html5&logoColor=white)]()

**App de Reservas de Manicura** es una solución de software comercial orientada a pequeños negocios de estética y belleza. Ofrece un flujo doble de reserva pública para clientes desde dispositivos móviles y un panel de administración privado para la gestión de agenda del establecimiento.

> 🔒 **Nota sobre el código fuente:** Repositorio de presentación (*Showcase*). La versión comercial desplegada y configuraciones de producción se mantienen en privado. Solicita una demo técnica para ver la app en ejecución.

---

## 🎯 Características Principales

### 1. 📱 Portal de Reservas para Clientes (Mobile-First)
* **Selección de Tratamientos:** Catálogo de servicios con duraciones y precios dinámicos.
* **Reserva de Horarios:** Selección de fecha y franja horaria disponible en tiempo real.
* **Confirmación de Cita:** Formulario sencillo sin fricción de registro largo.

### 2. 🔐 Panel de Control de Administración (Privado)
* **Gestión de Agenda:** Visualización diaria y semanal de las citas programadas.
* **CRUD de Tratamientos:** Alta, baja y modificación de precios, duraciones y descripciones de servicios.
* **Cancelación & Notificación:** Control total de horarios bloqueados y citas activas.

---

## 🛠️ Arquitectura de Software

```mermaid
graph TD
    A[Cliente Móvil - Web UI] -->|Reserva de Cita| B[FastAPI Backend - Python]
    C[Dueña / Admin Panel] -->|Gestión de Agenda & Precios| B
    B -->|Consultas SQLAlchemy| D[Base de Datos Relacional SQLite]
```

### 💻 Stack Tecnológico
* **Backend:** **FastAPI** (Python 3.8+) con **Uvicorn**.
* **Base de Datos:** **SQLite** con **SQLAlchemy ORM**.
* **Frontend:** **HTML5, CSS3, JavaScript Vanilla** optimizado para carga ultra rápida en teléfonos móviles.
