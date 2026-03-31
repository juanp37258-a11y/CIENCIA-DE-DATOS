i# 📊 Mi Portafolio de Ciencia de Datos

¡Bienvenido! Soy **Juan Pablo** y aquí comparto mis proyectos y trabajos en ciencia de datos.

## 📌 Introducción

Este repositorio contiene una **colección completa y progresiva de proyectos, scripts educativos y recursos profesionales** relacionados con **Ciencia de Datos**, **Análisis de Información** y **Visualización de Datos**. 

### 🎯 Objetivo del Portafolio

Mi objetivo es documentar y compartir mi trayecto de aprendizaje en ciencia de datos, desde conceptos fundamentales hasta análisis complejos de datasets reales. Este portafolio incluye:

- **5 clases prácticas** (`clase_1.py`, `clase_2.py`, `clase_3.py`, `clase_4.py`, `clase_5.py`) que cubren desde fundamentos hasta temas avanzados
- **Proyectos evaluados** (`parcial.py`, `trabajocustomers.py`) con análisis reales de datos de clientes
- **Visualizaciones profesionales** (`poster.py`, `power_bi.png`, `poster.jpeg`) para comunicar resultados efectivamente

### 📚 Contenido Principal

Este repositorio está estructurado en tres pilares:

1. **Formación Académica**: Series de lecciones progresivas en Python aplicadas a ciencia de datos
2. **Proyectos Prácticos**: Casos reales de análisis de datos con limpieza, exploración y segmentación
3. **Visualización y Comunicación**: Herramientas para generar dashboards e informes profesionales

Aquí encontrarás desde ejercicios prácticos fundamentales hasta análisis complejos de datasets reales, con énfasis en la **interpretación de resultados** y la **comunicación de insights**.

---

## 📁 Archivos del Repositorio

### 📚 Clases - Cursos Prácticos

| Archivo           | Descripción                                                                                                               |
|-------------------|---------------------------------------------------------------------------------------------------------------------------|
| **clase_1.py**     | Fundamentos de Data Science: NumPy, Pandas y Matplotlib básico. Introducción a arrays, matrices y gráficas simples. Además, se incluyen ejemplos de simulación como un generador de dados y juego de cartas usando NumPy. |
| **clase_2.py**     | Manipulación avanzada de datos con Pandas: Series, DataFrames, filtros con loc e iloc, y exportación de datos a CSV, HTML, JSON. Incluye creación y manipulación de columnas de DataFrames para cálculos estadísticos básicos. |
| **clase_3.py**     | Visualización de datos con Matplotlib: gráficos de línea, histogramas, boxplots y análisis exploratorio visual. (Archivo pendiente de recuperación). |
| **clase_4.py**     | Análisis exploratorio de datos (EDA) avanzado con datasets reales de crédito bancario y visualizaciones con Seaborn. (Archivo pendiente de recuperación). |
| **clase_5.py**     | Temas avanzados: aplicaciones prácticas de ciencia de datos, modelado estadístico y técnicas de predicción. (Archivo pendiente de recuperación). |

### 📊 Proyectos y Evaluaciones

| Archivo                    | Descripción                                                                                                                          |
|----------------------------|--------------------------------------------------------------------------------------------------------------------------------------|
| **trabajocustomers.py**     | Análisis completo de datos de clientes: limpieza, exploración, segmentación y visualización de patrones de comportamiento. El proyecto incluye gráficos avanzados para analizar la mediana y moda de los ingresos por género. |
| **parcial.py**              | Generación de un dataset sintético de clientes, análisis de correlación entre nivel educativo, salario y aprobación de crédito. Incluye visualizaciones como histogramas y boxplots para explorar outliers y tendencias. |
| **poster.py**               | Script para generar visualizaciones de resumen y posters informativos del proyecto con resultados principales. (Archivo pendiente de recuperación). |

### 🎨 Recursos Visuales

| Archivo        | Descripción                                                                                   |
|----------------|-----------------------------------------------------------------------------------------------|
| **poster.jpeg** | Imagen resumen del proyecto con resultados principales, gráficos y hallazgos clave.           |
| **power_bi.png**| Dashboard interactivo creado en Power BI con análisis visual, KPIs y métricas de negocio.      |

---

## 🛠️ Tecnologías Utilizadas

- **Python 3** — lenguaje principal
- **NumPy** — computación numérica
- **Pandas** — manipulación y análisis de datos
- **Matplotlib** — visualización básica
- **Seaborn** — visualización estadística avanzada
- **Power BI** — dashboards interactivos
- **Jupyter Notebook** — análisis interactivo

---
🟩 clase_1.py
Fundamentos de Data Science con Python: arrays, simulaciones y visualización de datos.
📖 Temas:
NumPy — creación de arrays, matrices y operaciones con np.array, np.eye
Aleatoriedad — generación de números con np.random.rand y np.random.randint
Juego de Dados — simulación de tiradas con resultados enteros
Juego de Cartas — representación de mazos con arrays 2D
Matplotlib — graficación de vectores, matrices y curvas con variación aleatoria
Pandas — primeros pasos con Series y DataFrame
⚡ Actividad:
# 🎲 Simulación de dado
dado = np.random.randint(low=1, high=7)

# 🃏 Mazo de cartas con arrays
all_cards = np.array([pikas, trebol, diamante, corazon])

# 📈 Curva de crecimiento con variación aleatoria
crecimiento = edad * 6 + np.random.randn(len(edad)) * 2
plt.plot(edad, crecimiento, marker='o', linestyle='-')
plt.title('Crecimiento a lo largo del tiempo')
plt.show()

🟦 clase_2.py
Introducción profunda a Pandas: Series, DataFrames y manipulación de datos tabulares.
📖 Temas:
Pandas — instalación y configuración con pyarrow
Series — creación con índices y valores personalizados
DataFrame — estructuras de datos tabulares
Manipulación — filtros, selección de columnas con loc e iloc
Exportación — guardado de datos en .csv, .html, .json
⚡ Actividad:
# 📊 Serie básica de Pandas
s = pd.Series([2, 4, 6, 8, 10])

# 🗂️ DataFrame de personas
personas = {
    "peso":   pd.Series([84, 90, 56, 64]),
    "altura": pd.Series([187, 170, 160, 155]),
    "hijos":  pd.Series([2, 3, 1, 0])
}
df = pd.DataFrame(personas)
⚙️ Requisitos:
pip install pandas pyarrow

