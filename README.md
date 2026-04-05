# 🏠 EDA — Ames Housing Dataset
> Análisis Exploratorio de Datos completo sobre 1.460 viviendas en Ames, Iowa.

---

## 📌 Descripción

Este proyecto aplica una metodología de **Análisis Exploratorio de Datos (EDA)** sobre el dataset de precios de viviendas de Ames, Iowa — el mismo proceso que utilizo en mi trabajo diario como analista de datos para evaluar información de terceros antes de que ingrese a una base de datos.

Desarrollado como parte del curso **Python para Ciencia de Datos** en A2Capacitación, con foco en buenas prácticas de análisis, visualización e interpretación de resultados.

---

## 🎯 Objetivos

- Comprender la estructura y calidad del dataset antes de modelar
- Identificar los factores que más influyen en el precio de venta
- Detectar valores faltantes, outliers y variables redundantes
- Construir variables derivadas que mejoren la capacidad predictiva

---

## 🔍 Hallazgos Principales

| Hallazgo | Detalle |
|----------|---------|
| 🎯 Variable objetivo sesgada | `SalePrice` tiene sesgo positivo de 1.88 → corregido con transformación logarítmica |
| 🏆 La calidad supera al tamaño | `OverallQual` (r = 0.79) es más predictiva que el área habitable (r = 0.71) |
| 🔧 Feature Engineering efectivo | `TotalSF` (suma de todos los pisos) alcanza r = 0.782 con el precio |
| ⚠️ Nulos que no son errores | 19 columnas con vacíos que representan ausencia de característica, no datos perdidos |
| 🔗 Multicolinealidad detectada | `GarageCars` ↔ `GarageArea` con r = 0.88 — redundancia a resolver antes de modelar |

---

## 📁 Estructura del Repositorio

```
eda-ames-housing/
│
├── EDA_Housing_Profesional_ES.ipynb   # Notebook principal con el análisis completo
├── README.md                          # Este archivo
└── train.csv                          # Dataset original (Kaggle)
```

---

## 🛠️ Herramientas y Librerías

| Herramienta | Uso |
|-------------|-----|
| `Python 3` | Lenguaje base |
| `Pandas` | Manipulación y limpieza de datos |
| `NumPy` | Operaciones numéricas |
| `Matplotlib` | Visualizaciones base |
| `Seaborn` | Visualizaciones estadísticas |
| `SciPy` | Pruebas estadísticas (Shapiro-Wilk, skewness) |

---

## 📊 Contenido del Notebook

1. Configuración inicial y paleta de colores
2. Carga e inspección del dataset
3. Análisis de valores faltantes
4. Distribución de la variable objetivo `SalePrice`
5. Análisis de correlaciones y heatmap
6. Distribución de variables numéricas clave
7. Análisis de variables categóricas
8. Análisis bivariado detallado
9. Detección de outliers (método IQR)
10. Ingeniería de variables (Feature Engineering)
11. Análisis de multicolinealidad
12. Patrones temporales de ventas
13. Análisis de sesgo (Skewness)
14. Hallazgos clave y recomendaciones para modelado

---

## 📂 Dataset

- **Fuente:** [Kaggle — House Prices: Advanced Regression Techniques](https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques)
- **Registros:** 1.460 propiedades
- **Variables:** 81 (38 numéricas, 43 categóricas)
- **Período:** 2006 – 2010

---

## 👤 Autor

**Jordan Aramis**
Analista de Datos
[LinkedIn](https://www.linkedin.com/in/) · [GitHub](https://github.com/JordanAramis)

