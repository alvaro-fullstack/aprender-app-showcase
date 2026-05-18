# 🔍 LikeTurnitin — Calibrador de Precisión & Detector de Plagio IA para Textos Académicos

[![Python](https://img.shields.io/badge/Python-3.10+-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)
[![NLP](https://img.shields.io/badge/NLP-Natural_Language_Processing-FF6F61?style=for-the-badge&logo=nlp&logoColor=white)]()
[![JSON Schema](https://img.shields.io/badge/JSON_Schema-Validation-000000?style=for-the-badge&logo=json&logoColor=white)]()

**LikeTurnitin** es un motor de análisis lingüístico avanzado y calibrador de detección de plagio por Inteligencia Artificial diseñado específicamente para documentos académicos extensos en español (como Trabajos de Fin de Grado — TFG y Trabajos de Fin de Máster — TFM). 

El objetivo primordial del sistema es replicar con precisión milimétrica los comportamientos de detección de herramientas líderes en el sector educativo, alcanzando una paridad calibrada del **41% de detección de IA**.

> 🔒 **Nota sobre el código fuente:** Este es un repositorio público de presentación (*Showcase*). El código fuente del motor de análisis en Python (`ai_detector.py`), los datasets de prueba y el archivo de calibración `ground_truth.json` se encuentran en un **repositorio privado** para proteger la propiedad intelectual y evitar la elusión de detectores académicos. Si deseas una revisión del código fuente, por favor contáctame para una demo por pantalla compartida.

---

## 🔬 Ingeniería Lingüística & Características del Motor

### 1. 🎯 Calibración de Paridad (Exactitud del 41%)
*   **El Reto:** Los detectores comerciales como Turnitin no analizan oraciones aisladas; evalúan patrones de escritura globales. Muchos detectores open-source sufren de falsos positivos o negativos al procesar español académico.
*   **La Solución:** Un motor heurístico calibrado frente a un dataset validado por humanos (`ground_truth.json`). El sistema optimiza dinámicamente sus umbrales de confianza para ajustarse exactamente al 41% de detección requerido, asegurando que los bloques marcados coincidan exactamente con la realidad del comportamiento del software de inspección docente.

### 2. 🛡️ Filtrado Inteligente de Plantillas y Cabeceras
*   **Funcionalidad:** Evita falsos positivos en las secciones críticas no redactadas por el estudiante.
*   **Implementación:** Filtra algoritmicamente:
    *   Portadas oficiales y logotipos universitarios.
    *   Cabeceras académicas y pies de página.
    *   Firmas de tribunales y portadas de entrega.
    *   Citas bibliográficas normativas.

### 3. 📈 Detección Contigua por Bloques
*   **Funcionalidad:** En lugar de resaltar palabras o frases sueltas (lo cual resulta ilegible y poco útil), el algoritmo agrupa oraciones con alta probabilidad de autoría por IA para resaltar **párrafos contiguos y fluidos**, idéntico a cómo presenta los informes Turnitin.
*   **Algoritmo:** Implementa un analizador de ventanas deslizantes que evalúa la densidad de la probabilidad de IA en bloques de texto adyacentes para consolidar áreas marcadas.

---

## 🛠️ Arquitectura Técnica & Dataset de Validación

El motor de análisis está optimizado para procesar texto plano y estructurado bajo una lógica de flujo de datos muy rigurosa:

```mermaid
graph LR
    A[Documento Académico TFM] --> B[Filtro de Cabeceras & Bibliografía]
    B --> C[Segmentación por Párrafos]
    C --> D[Motor de Detección Heurístico]
    D -->|Validación cruzada| E[ground_truth.json]
    E --> F[Consolidación de Bloques Contiguos]
    F --> G[Informe de Similitud - 41% Paridad]
```

### 💻 Stack de Ingeniería
*   **Python 3.10+:** Lenguaje núcleo para procesamiento de datos y NLP.
*   **Heurísticas de NLP:** Algoritmos de análisis de perplejidad y burstiness (variabilidad de escritura) adaptados a las particularidades del español académico.
*   **Ground Truth Engine:** Sistema de pruebas unitarias y regresión basado en JSON que valida cada ajuste del algoritmo contra un histórico de documentos de prueba para asegurar que los cambios en el código no alteren la precisión del calibrador general.

---

## 📈 Metodologías de Desarrollo Aplicadas

1.  **Desarrollo Basado en Datos (Data-Driven Calibration):** Calibración constante del motor iterando el código de `ai_detector.py` y comparando el output matemático contra las anotaciones reales del dataset de control.
2.  **Robustez Lingüística:** Tratamiento exhaustivo de caracteres especiales del español (tildes, eñes, diéresis) y estructuras gramaticales complejas típicas de textos de postgrado.
