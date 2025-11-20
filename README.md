# Análisis Predictivo de Cancelaciones en Reservas Hoteleras

![Banner o captura del dashboard](powerbi/screenshots/dashboard_overview.png)

## 🎯 Objetivo
Predecir la probabilidad de cancelación de reservas hoteleras utilizando Random Forest y crear un dashboard ejecutivo en Power BI.

## 📊 Dataset
- Fuente: [Hotel booking demand (Kaggle)](https://www.kaggle.com/datasets/jessemostipak/hotel-booking-demand)
- 119.390 observaciones, 32 variables

## 🔮 Modelo
- Algoritmo: Random Forest Classifier
- AUC-ROC: 0.89 | Accuracy: 87% | Recall (cancelaciones): 82%
- Feature importance destacada: `lead_time`, `deposit_type`, `country`, etc.

## 📈 Dashboard Ejecutivo en Power BI
![Dashboard](powerbi/screenshots/dashboard_overview.png)
[Ver más capturas](powerbi/screenshots/)

## Estructura del proyecto
(árbol de carpetas aquí)

## 🚀 Cómo ejecutar
```bash
conda env create -f environment.yml
conda activate hotel-cancellation
jupyter notebook notebooks/

Yeison Vela - www.linkedin.com/in/yeison-vela
