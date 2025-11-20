👨‍💻 Autor
Yeison Vela
Data Scientist | Especialista en Análisis Predictivo
www.linkedin.com/in/yeison-vela | yeiasvs@gmail.com

# Análisis Predictivo de Cancelaciones en Reservas Hoteleras  
**Random Forest + Dashboard Ejecutivo en Power BI**

![Dashboard Preview](powerbi/screenshots/01_dashboard_general.png)

## 🎯 Objetivo del proyecto
Desarrollar un modelo de Machine Learning capaz de predecir con alta precisión si una reserva hotelera será cancelada o no, y entregar un **dashboard ejecutivo en Power BI** para que el área de Revenue Management pueda tomar decisiones en tiempo real.

**Resultados del modelo (Random Forest):**
- Accuracy: **87.4%**
- AUC-ROC: **0.94**
- Recall (detección de cancelaciones): **83%**

## 📊 Dataset
- Fuente: [Hotel booking demand - Kaggle](https://www.kaggle.com/datasets/jessemostipak/hotel-booking-demand)
- 119.390 reservas de dos hoteles (City & Resort) entre 2015-2017
- Variable objetivo: `is_canceled` (0 = No cancelada, 1 = Cancelada → 37% de cancelaciones)

## 🧠 Modelo y características más importantes
![Feature Importance](reports/figures/feature_importance.png)

Las variables con mayor poder predictivo son:
1. `lead_time` (tiempo de antelación)
2. `deposit_type` (tipo de depósito)
3. `country` (país de origen)
4. `total_of_special_requests`
5. `required_car_parking_spaces`

## 📈 Dashboard Ejecutivo en Power BI
![Dashboard](powerbi/screenshots/02_tasa_cancelacion.png)

Características del dashboard:
- Tasa de cancelación por mes, tipo de hotel, canal de venta y país
- Predicciones del modelo integradas (script Python en Power BI)
- Segmentación interactiva y KPIs clave
- Alertas visuales para períodos de alto riesgo

## 🚀 Cómo ejecutar el proyecto (100% reproducible)

```bash
# 1. Clonar el repo
git clone https://github.com/tu-usuario/Hotel-Cancellation-Prediction.git
cd Hotel-Cancellation-Prediction

# 2. Crear entorno
pip install -r requirements.txt

# 3. Ejecutar todo el pipeline (EDA + entrenamiento + gráficas)
python main.py

# 4. Abrir el notebook (opcional)
jupyter notebook notebooks/01_Analisis_Exploratorio_y_Modelo.ipynb

# 5. Abrir el dashboard
powerbi/Hotel_Cancellation_Dashboard.pbix
