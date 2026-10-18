# Changelog — Actividad 5

## 0.2.0 — Dataset etiquetado
- Incorporación de anotaciones YOLO para `smoke` y `fire`.
- Incorporación de ejemplos negativos de nubes.
- Validación estructural de imágenes y etiquetas.

## 0.1.0 — Dataset inicial
- Versionado de los fotogramas seleccionados antes del etiquetado.
- Conservación del manifiesto de procedencia.

## Experimentos
- Comparación de YOLOv8s ajustado con Wildfire y datos privados de DVR.
- Registro de experimentos y métricas en MLflow.
- Trabajo futuro: aumentar los positivos y reducir falsas alarmas por
  nubes y niebla sin perder sensibilidad ante incendios reales.
