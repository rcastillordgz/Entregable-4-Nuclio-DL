# 🚀 Proyecto de Transfer Learning y Diseño de CNN desde Cero

## 📋 Descripción

Este proyecto explora distintas estrategias para la clasificación de imágenes del dataset **CIFAR100** utilizando técnicas de **Transfer Learning** y **arquitecturas diseñadas desde cero**.

Se han trabajado tres enfoques principales:

- **ResNet50 Fine-Tuned**: Transfer Learning con modelo preentrenado en ImageNet, seguido de fine-tuning.
- **MobileNetV2 Fine-Tuned**: Transfer Learning con un modelo ligero, optimizado para eficiencia.
- **Custom CNN Potente**: Red neuronal convolucional construida desde cero, utilizando técnicas de optimización avanzadas (BatchNormalization, Dropout, ReduceLROnPlateau).

---

## 🛠️ Estructura del proyecto

- `notebooks/`: Cuadernos de Google Colab con todo el proceso documentado.
- `README.md`: Documento actual.

> ❗ No se han guardado figuras gráficas (`.png`). Todas las visualizaciones se encuentran en los notebooks.
> ❗ No se han guardado modelos (`.h5`) por su tamaño.
> ❗ No se han guardado los historiales (`.pkl`) por su tamaño.
> 📢 Si se desean guardar, recomendamos ejecutar el notebook y guardarlos en local.

---

## 📈 Resultados

### 📊 Comparativa de modelos

| Modelo                 | Val Accuracy Final | Val Loss Final | Tamaño (.h5) | Tiempo Entrenamiento | Épocas Totales | Comentario Principal |
|-------------------------|--------------------|----------------|--------------|----------------------|----------------|----------------------|
| **ResNet50 Fine-Tuned**  | 75.3%              | ~1.00          | 165 MB       | ~1 hora              | 20 + 8         | Muy precisa, pesada y lenta. |
| **MobileNetV2 Fine-Tuned** | 71.6%             | ~1.35          | 14 MB        | ~15 minutos          | 10             | Muy eficiente, rápida, ligera. |
| **Custom CNN Potente**   | 45.2%              | ~2.51          | ~35 MB       | ~25 minutos          | 26             | Buen desempeño para ser diseñada desde cero. |

---

## 🧠 Conclusiones

- **ResNet50 Fine-Tuned** es la mejor opción en cuanto a precisión, ideal para entornos donde los recursos computacionales no son una limitación.
- **MobileNetV2 Fine-Tuned** ofrece un equilibrio óptimo entre rendimiento y eficiencia, siendo muy adecuado para aplicaciones en dispositivos móviles o con restricciones de hardware.
- **Custom CNN Potente** demuestra que **con un diseño cuidadoso**, una CNN desde cero puede ser competitiva, consiguiendo una performance sólida con un coste computacional moderado.

> 📢 **Nota importante**: La evolución de los modelos está completamente documentada en el notebook, mostrando todo el proceso iterativo de mejora y toma de decisiones.

---

## 🚀 Tecnologías utilizadas

- TensorFlow 2.x
- Keras
- Python 3
- Google Colab
- Matplotlib
- Scikit-Learn

---

## 📂 Cómo reproducir

1. Cargar los notebooks de entrenamiento en Google Colab.
2. Asegurar que tienes acceso a GPU (preferiblemente A100 o L4 si tienes Colab Pro).
3. Ejecutar las celdas en orden: carga de datos → preprocesamiento → definición de modelo → entrenamiento → evaluación.
4. Visualizar los resultados finales directamente en el notebook.

---

## 🏆 Créditos

Proyecto realizado por Ricardo Castillo Rodríguez
---
