# 🎮 EDA Steam Store Games

Análisis Exploratorio de Datos sobre el catálogo de Steam para identificar tendencias de mercado y factores que influyen en el éxito de un videojuego.

![Python](https://img.shields.io/badge/Python-3.11-blue?logo=python)
![Pandas](https://img.shields.io/badge/Pandas-2.x-150458?logo=pandas)
![Seaborn](https://img.shields.io/badge/Seaborn-0.x-4c72b0)
![Looker Studio](https://img.shields.io/badge/Looker%20Studio-Dashboard-4285F4?logo=googleanalytics)
![Dataset](https://img.shields.io/badge/Dataset-27.075%20juegos-green)

---

## 📌 Descripción

Steam es la plataforma de distribución de videojuegos para PC más grande del mundo. Este proyecto analiza su catálogo con una metodología orientada a preguntas de negocio, siguiendo el flujo completo de un EDA profesional: carga, limpieza, análisis y visualización.

---

## ❓ Preguntas de Negocio

Las preguntas fueron definidas **antes** de explorar los datos:

1. ¿Cómo ha evolucionado la cantidad de juegos publicados por año?
2. ¿Qué géneros dominan el mercado y cuáles tienen mejor valoración?
3. ¿Existe relación entre el precio de un juego y su valoración?
4. ¿Qué desarrolladores tienen mejor ratio calidad-precio?
5. ¿Los juegos gratuitos tienen peor valoración que los de pago?

---

## 🔍 Hallazgos Principales

- 📈 El catálogo de Steam pasó de ~400 juegos en 2013 a **más de 8.000 en 2018**, impulsado por Steam Greenlight.
- 🎮 **Action** domina en cantidad pero **RPG** lidera en valoración media (71.6%).
- 💰 La correlación entre precio y valoración es de apenas **0.10** — el precio no determina la calidad.
- 🏆 Los estudios **indie** superan en ratio calidad-precio a los grandes estudios por un factor de **4-5x**.
- 🆓 Los juegos gratuitos (71.9%) y de pago (71.4%) tienen valoraciones **prácticamente idénticas**.

---

## 🗂️ Estructura del Proyecto

```
Proyecto-EDA-Steam-Store-Games/
│
├── Data/
│   ├── steam.csv                     ← Dataset principal (27.075 juegos)
│   ├── steamspy_tag_data.csv         ← Tags detallados por juego
│   ├── steam_limpio.csv              ← Dataset limpio exportado
│   ├── opcional/                     ← Archivos no utilizados en el análisis
│   └── no_necesario/
│
├── img/                              ← Visualizaciones generadas
│   ├── 01_juegos_por_año.png
│   ├── 02_top_generos_cantidad.png
│   ├── 03_valoracion_por_genero.png
│   ├── 04_precio_vs_valoracion.png
│   ├── 05_precio_vs_valoracion_tendencia.png
│   ├── 06_top_devs_calidad_precio.png
│   ├── 07_top_grandes_estudios_calidad_precio.png
│   └── 08_gratuitos_vs_pago.png
│
├── steam_eda_esquema.ipynb           ← Introducción, objetivos y diccionario
├── steam_eda.ipynb                   ← Análisis principal
├── EDA_Steam_Store_Games_Lucas_Balaguer.docx  ← Informe completo
└── README.md
```

---

## 📊 Dashboard Interactivo

El análisis incluye un dashboard interactivo desarrollado en **Looker Studio**:

🔗 [Ver Dashboard en Looker Studio](https://datastudio.google.com/reporting/ab6719b0-4b61-44e4-8cf1-93a09eb5ac91)

---

## 🛠️ Tecnologías Utilizadas

| Herramienta | Uso |
|---|---|
| Python 3.11 | Lenguaje principal |
| Pandas | Carga, limpieza y manipulación de datos |
| Matplotlib | Visualizaciones base |
| Seaborn | Visualizaciones estadísticas |
| Looker Studio | Dashboard interactivo |
| VSCode + Jupyter | Entorno de desarrollo |

---

## 📦 Dataset

**Fuente:** [Kaggle - Steam Store Games](https://www.kaggle.com/datasets/nikdavis/steam-store-games)  
**Origen:** SteamSpy API + Steam Store API  
**Fecha de extracción:** Mayo 2019  
**Licencia:** CC0 (Dominio público)  
**Registros:** 27.075 juegos · 18 variables originales

---

## 🚀 Cómo Ejecutar el Proyecto

1. Clona el repositorio:
```bash
git clone https://github.com/LucasBalaguer/Proyecto-EDA-Steam-Store-Games.git
```

2. Instala las dependencias:
```bash
pip install pandas matplotlib seaborn jupyter
```

3. Abre los notebooks en orden:
   - Primero `steam_eda_esquema.ipynb` para el contexto del proyecto
   - Luego `steam_eda.ipynb` para el análisis completo

---

## 👤 Autor

**Lucas Balaguer**  
Data Analyst · Bootcamp Data Science & IA — The Bridge (2025-2026)

[![LinkedIn](https://img.shields.io/badge/LinkedIn-lucas--cavalcante--balaguer-0077B5?logo=linkedin)](https://www.linkedin.com/in/lucas-cavalcante-balaguer)
[![GitHub](https://img.shields.io/badge/GitHub-LucasBalaguer-181717?logo=github)](https://github.com/LucasBalaguer)