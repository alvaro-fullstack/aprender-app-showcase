# 🧩 DevLens / Console Log Ninja — Extensión de Depuración Visual para VS Code

[![TypeScript](https://img.shields.io/badge/TypeScript-Extension-3178C6?style=for-the-badge&logo=typescript&logoColor=white)](https://www.typescriptlang.org/)
[![VS Code](https://img.shields.io/badge/VS_Code-API-007ACC?style=for-the-badge&logo=visualstudiocode&logoColor=white)](https://code.visualstudio.com/)
[![Node.js](https://img.shields.io/badge/Node.js-18+-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)](https://nodejs.org/)

**DevLens / Console Log Ninja** es una extensión para Visual Studio Code diseñada para acelerar la depuración de código en entornos JavaScript y TypeScript mediante inserción automatizada de logs y análisis contextual de variables.

> 🔒 **Nota sobre el código fuente:** Repositorio de presentación (*Showcase*). El paquete de extensión `.vsix` y fuentes completas residen en un repositorio privado. Contacta con el autor para más información.

---

## 🎯 Características Principales

1. **Inserción de Logs en Un Clic:** Inserta comandos de log formateados profesionalmente con contexto de archivo, línea y nombre de variable.
2. **Limpieza Inteligente de Logs:** Elimina todos los `console.log` de depuración creados temporalmente antes de realizar commits.
3. **Análisis AST de Variables:** Utiliza el árbol de sintaxis abstracta (*Abstract Syntax Tree*) de TypeScript para identificar identificadores válidos.

---

## 🛠️ Arquitectura Técnica

* **Extensión API:** Integración nativa con la API de Visual Studio Code (`vscode.workspace`, `vscode.window`).
* **Lenguaje:** **TypeScript** compilado con `tsc` y empaquetado optimizado para el editor.
