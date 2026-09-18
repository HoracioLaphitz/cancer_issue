# Análisis Predictivo de Cáncer

## Descripción

> 🚧 Proyecto en desarrollo (en proceso).

## Estructura del proyecto

- `data/raw/` — datos de entrada.
- `notebooks/` — análisis exploratorio y experimentación.
- `src/` — código fuente del pipeline (procesamiento, entrenamiento, evaluación).
- `tests/` — suite de tests automatizados.
- `deployment/` — artefactos para despliegue del modelo.
- `reports/figures/` — visualizaciones generadas.
- `main.py` — punto de entrada del proyecto.
- `requirements.txt` — dependencias.

## Metodología (objetivos de diseño)

El proyecto está pensado para cubrir las siguientes etapas:

- Análisis exploratorio de datos (univariado, multivariado, PCA).
- Ingeniería de características y balanceo de clases.
- Comparación de modelos: regresión logística, Random Forest, XGBoost, SVM, redes neuronales.
- Optimización de hiperparámetros (Grid Search / Random Search / Optuna).
- Evaluación con métricas estándar (accuracy, precision, recall, F1, ROC-AUC) y matriz de confusión.
- Interpretabilidad de resultados (SHAP).

> **Nota sobre métricas:** las cifras de performance y de impacto de negocio no están incluidas en este README porque, al día de esta actualización, no pudieron verificarse contra resultados reproducibles del repositorio (no hay un `metrics.json` u output de evaluación consultado). Los puntos anteriores describen los objetivos de diseño del pipeline, no resultados medidos. Cuando el proyecto tenga una corrida de evaluación reproducible, esta sección puede actualizarse con las cifras reales y su fuente.

## Diagrama

[Explorar la arquitectura interactiva en GitDiagram](https://gitdiagram.com/HoracioLaphitz/cancer_issue)

```mermaid
flowchart LR
  A["data + deployment + logs"] --> B["Procesamiento de cancer_issue"]
  B --> C["Resultados del proyecto"]
```

## Tecnologías

Python · scikit-learn · XGBoost · SHAP · pytest

## Cómo ejecutar

```bash
pip install -r requirements.txt
python main.py
```

## Autor

Horacio Laphitz — [GitHub](https://github.com/HoracioLaphitz) · [LinkedIn](https://www.linkedin.com/in/horacio-laphitz)
