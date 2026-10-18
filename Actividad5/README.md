# Actividad 5 — Sylva AI

## Objetivo
Desarrollar y evaluar un detector de fuego y humo forestal con YOLOv8,
utilizando datos públicos de incendios y ejemplos de cámaras DVR.

## Estructura
- `datos/datos_ini/`: versión inicial de los fotogramas seleccionados.
- `datos/datos_limp/`: imágenes preparadas y anotaciones YOLO.
- `fuentes/entrena.ipynb`: experimentos, entrenamiento y evaluación.
- `fuentes/datos_prep.py`: auditoría de la estructura y etiquetas.
- `fuentes/train.py`: script de entrenamiento con registro en MLflow.

## Clases
- `0`: smoke
- `1`: fire

## Reproducibilidad
1. Configurar un entorno Python compatible con la versión de Ultralytics.
2. Auditar los datos utilizando `datos_prep.py`.
3. Preparar el archivo `data.yaml` con particiones de entrenamiento y validación.
4. Ejecutar `train.py` con los pesos iniciales y el YAML correspondiente.
5. Consultar los experimentos y las métricas en MLflow.

## Decisiones técnicas
Se mantienen ejemplos negativos de nubes y otras condiciones ambientales
para estudiar la reducción de falsas alarmas. La selección del modelo deberá
considerar recall por clase, mAP, latencia y falsas alarmas en vídeos
independientes.

Las grabaciones originales completas de los DVR no se incluyen en este
repositorio. Los datos versionados son fotogramas seleccionados.
