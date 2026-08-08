# 🎮 Tower of Elements & JuegosRaiz — Videojuegos 3D Web & IA Multi-Agente (MARL)

[![Three.js](https://img.shields.io/badge/Three.js-WebGL-000000?style=for-the-badge&logo=three.js&logoColor=white)](https://threejs.org/)
[![React Three Fiber](https://img.shields.io/badge/React_Three_Fiber-3D-61DAFB?style=for-the-badge&logo=react&logoColor=black)](https://docs.pmnd.rs/react-three-fiber)
[![TypeScript](https://img.shields.io/badge/TypeScript-Strict-3178C6?style=for-the-badge&logo=typescript&logoColor=white)](https://www.typescriptlang.org/)
[![PyTorch](https://img.shields.io/badge/PyTorch-MARL_AI-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white)](https://pytorch.org/)

**Tower of Elements & JuegosRaiz** es un proyecto enfocado en la exploración gráfica 3D en la web mediante WebGL e Inteligencia Artificial basada en Aprendizaje por Refuerzo Multi-Agente (MARL).

> 🔒 **Nota sobre el código fuente:** Repositorio de presentación (*Showcase*). Los assets 3D optimizados, modelos entrenados de redes neuronales `.pt` y repositorios de motores se mantienen en privado. Solicita una demo técnica por pantalla compartida.

---

## 🎯 Proyectos Incluidos

### 1. ⚔️ Tower of Elements (Juego 3D WebGL)
* **Visuales Toon Shading:** Renderizado estilizado de personajes anime y escenarios mediante shaders personalizados (`BaseToonMaterial`).
* **Control & Físicas:** Movimiento de personajes 3D, combate, sistema de cámara y animaciones jerárquicas ejecutadas a 60 FPS estables en el navegador.
* **Stack:** `React 18`, `TypeScript`, `@react-three/fiber`, `@react-three/drei`, `Three.js`, `Vite`.

### 2. ⚽ Soccer-Gemini (Aprendizaje por Refuerzo Multi-Agente - MARL)
* **Entorno de Simulación:** Simulación deportiva en Python donde múltiples agentes compiten y colaboran en tiempo real.
* **Algoritmos de IA:** Redes neuronales profundas entrenadas con PyTorch e interfaces de aprendizaje de entornos tipo Gymnasium / PettingZoo.

---

## 🛠️ Arquitectura Gráfica & Flujo de Simulación

```mermaid
graph TD
    subgraph "Tower of Elements (Frontend 3D WebGL)"
        A[React Three Fiber Canvas] --> B[Escena 3D & Toon Shading Materials]
        B --> C[Modelos GLTF / GLB Character Render]
        C --> D[Render Loop 60 FPS]
    end

    subgraph "Soccer-Gemini (IA PyTorch MARL)"
        E[Environment Gymnasium / PettingZoo] --> F[Agentes Autónomos Redes Neuronales]
        F -->|Recompensas & Observaciones| G[Entrenamiento PyTorch MARL Pipeline]
    end
```
