### **Deep Learning - Maestría Management & Analytics**

# **Extracción Automatizada de Información en Cartas Documento Bancarias: Comparación de Técnicas OCR vs GPT-5**


## 1. Problema a Resolver
Este proyecto busca dar los primeros pasos en la creación de un agente que responda cartas documento enviadas a instituciones bancarias. 
El objetivo es determinar cual es el mejor método de OCR para digitalizar este tipo de documentos. Es por ello que probaremos distintos enfoques y desarrollaremos una métrica de evaluación.

## 2. Dataset

* Fuentes públicas **PJN** (pjn.gov.ar).
* CDs en PDF/imágenes, resoluciones variadas (200‑600 dpi).
* Rotación, ruido, sellos y firmas incluidas.


## 3. Herramientas analizadas

| Etapa | Herramienta        | Modelo subyacente                  |
| ----- | ------------------ | ---------------------------------- |
| OCR 1 | **Tesseract 5**    | LSTM bidireccional                 |
| OCR 2 | **Doctr**          | CNN + CTC / Transformer            |
| OCR 3 | **LLM multimodal** | GPT-5 |

Métrica de evaluación: cadenas de Levenshtein

## 4. Indice del repositorio
    1. Presentación general del trabajo.
    2. OCR con Tesseract (archivo readme disponible con requerimientos de sistema) + extracción de entidades con Llama 3
    3. OCR con Doctr (readme disponible con requerimientos de sistema) + extracción de entidades con Llama 3.
    4. Transcripción con modelo multimodal (GPT-5) + extracción de entidades con Llama 3.
    5. Evaluación con cadenas de Levenshtein + conclusión general.

## 5. Entregables
* Carpeta con Cartas Documento de ejemplo
* Notebook para probar Tesseract, Doctr y lectura con LLM (GPT-5 vía API) con VS Code – Windows.
* README con requisitos y uso de cada notebook.
* CSV resumen con variables extraídas con cada método.
* Carpeta con transcripción manual de muestra de cartas para evaluar.
* Notebook de evaluación utilizando cadenas de Levenshtein.
* Informe final con conclusiones y recomendaciones.
