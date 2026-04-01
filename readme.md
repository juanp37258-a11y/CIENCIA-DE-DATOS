# 📊 Portafolio de Ciencia de Datos — Juan Pablo

[![Python](https://img.shields.io/badge/Python-3.x-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)
[![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)](https://numpy.org/)
[![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)](https://pandas.pydata.org/)
[![Matplotlib](https://img.shields.io/badge/Matplotlib-11557c?style=for-the-badge)](https://matplotlib.org/)
[![Seaborn](https://img.shields.io/badge/Seaborn-4c9be8?style=for-the-badge)](https://seaborn.pydata.org/)
[![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)](https://powerbi.microsoft.com/)

---

## 🧭 Tabla de Contenidos

- [Introducción](#-introducción)
- [Archivos del Repositorio](#-archivos-del-repositorio)
- [Clase 1 — NumPy, Pandas y Matplotlib](#-clase-1--numpy-pandas-y-matplotlib)
- [Clase 2 — Pandas Avanzado](#-clase-2--pandas-avanzado)
- [Clase 3 — Visualización con Matplotlib](#-clase-3--visualización-con-matplotlib)
- [Clase 4 — Análisis Exploratorio EDA](#-clase-4--análisis-exploratorio-eda)
- [Clase 5 — Estadística Descriptiva](#-clase-5--estadística-descriptiva-y-visualización)
- [Proyectos y Evaluaciones](#-proyectos-y-evaluaciones)
- [Tecnologías](#️-tecnologías-utilizadas)
- [Instalación](#-instalación)

---

## 📌 Introducción

Bienvenido a mi portafolio de Ciencia de Datos. Aquí documento mi trayecto de aprendizaje en Python aplicado al análisis de datos, desde fundamentos hasta proyectos con datasets reales.

El portafolio se organiza en tres pilares:

| Pilar | Descripción |
|-------|-------------|
| 🎓 Formación Académica | Lecciones progresivas en Python aplicadas a ciencia de datos |
| 🔬 Proyectos Prácticos | Análisis reales con limpieza, exploración y segmentación |
| 📢 Visualización | Dashboards e informes que comunican resultados |

---

## 📁 Archivos del Repositorio

### Clases

| Archivo | Descripción |
|---------|-------------|
| clase_1.py | Fundamentos: NumPy, Pandas y Matplotlib básico. Arrays, simulaciones y primeras gráficas. |
| clase_2.py | Pandas avanzado: Series, DataFrames, filtros con loc e iloc, exportación a CSV, HTML y JSON. |
| clase_3.py | Visualización con Matplotlib: líneas, histogramas, scatter, subplots y guardado de figuras. |
| clase_4.py | EDA con dataset real de tarjetas de crédito: limpieza, nulos, value_counts y boxplots. |
| clase_5.py | Estadística descriptiva: media, mediana, IQR, outliers con regla de Tukey y comparativas. |

### Proyectos

| Archivo | Descripción |
|---------|-------------|
| trabajocustomers.py | Análisis completo de clientes: segmentación, patrones de comportamiento e ingresos por género. |
| parcial.py | Dataset sintético de clientes: correlación entre educación, salario y aprobación de crédito. |
| poster.py | Script generador de visualizaciones resumen con los hallazgos principales del portafolio. |

### Recursos Visuales

| Archivo | Descripción |
|---------|-------------|
| poster.jpeg | Imagen resumen con resultados, gráficos y hallazgos clave del proyecto. |
| power_bi.png | Dashboard interactivo creado en Power BI con KPIs y métricas de negocio. |

---

## 🟩 Clase 1 — NumPy, Pandas y Matplotlib

**Archivo:** `clase_1.py` | **Nivel:** Fundamentos

Introducción a los pilares del ecosistema de datos en Python.

**Temas cubiertos:**
- NumPy — arrays, matrices con `np.array` y `np.eye`
- Aleatoriedad — `np.random.rand` y `np.random.randint`
- Simulaciones — juego de dados y mazo de cartas con arrays 2D
- Matplotlib — vectores, matrices y curvas con variación aleatoria
- Pandas — primeros pasos con `Series` y `DataFrame`

**Código de ejemplo:**

```python
# Simulación de dado
dado = np.random.randint(low=1, high=7)

# Mazo de cartas
all_cards = np.array([pikas, trebol, diamante, corazon])

# Curva de crecimiento
crecimiento = edad * 6 + np.random.randn(len(edad)) * 2
plt.plot(edad, crecimiento, marker='o')
plt.show()

# DataFrame de estatura
datos_estatura = {
    "nombre": ["luis", "paco", "augusto"],
    "edad": [23, 34, 2],
    "estatura": [1.60, 1.69, 1.87]
}
df = pd.DataFrame(datos_estatura)
```

```bash
pip install numpy matplotlib pandas
```

---

## 🟦 Clase 2 — Pandas Avanzado

**Archivo:** `clase_2.py` | **Nivel:** Intermedio

Manipulación profunda de datos tabulares con Pandas.

**Temas cubiertos:**
- Series — índices y valores personalizados
- DataFrame — columnas múltiples y cálculos estadísticos
- Filtros — selección con `loc` e `iloc`
- Exportación — `.csv`, `.html`, `.json`

**Código de ejemplo:**

```python
# Serie básica
s = pd.Series([2, 4, 6, 8, 10])

# DataFrame
df = pd.DataFrame({'A': [1, 2, 3], 'B': [4, 5, 6], 'C': [2, 3, 4]})

# Exportar
df.to_csv("datos.csv")
df.to_html("datos.html")
df.to_json("datos.json")
```

```bash
pip install pandas pyarrow
```

---

## 🟨 Clase 3 — Visualización con Matplotlib

**Archivo:** `clase_3.py` | **Nivel:** Intermedio

Tipos de gráfico más utilizados en ciencia de datos.

**Temas cubiertos:**

| Sección | Descripción |
|---------|-------------|
| Gráfica de línea | Trazado de secuencias y curvas matemáticas |
| Parábola con NumPy | `np.linspace` para 500 puntos suaves |
| Múltiples líneas | Leyendas, grillas y estilos de línea |
| Subplots | Paneles múltiples con `plt.subplots` |
| Scatter | Dispersión con grupos de colores distintos |
| Histogramas | `bins` automáticos y manuales |
| Guardar figura | `fig.savefig()` con fondo transparente |

**Código de ejemplo:**

```python
# Múltiples líneas con leyenda
plt.plot(x, x**2, 'b--', label="x²")
plt.plot(x, x+1,  'g',   label="x+1")
plt.legend()
plt.grid()

# Subplots lado a lado
fig, ax = plt.subplots(1, 2, figsize=(14, 6))
ax[0].plot(x, y, 'r-', linewidth=3)
ax[0].set_title("Parábola", fontsize=16)
ax[0].grid(alpha=0.3)

# Guardar imagen
fig.savefig("mi_grafica.png", transparent=True)
```

```bash
pip install matplotlib numpy
```

---

## 🟥 Clase 4 — Análisis Exploratorio EDA

**Archivo:** `clase_4.py` | **Nivel:** Intermedio-Avanzado | **Dataset:** `credit_card.csv`

Exploración y limpieza de un dataset real de tarjetas de crédito.

**Columnas del dataset:**

| Columna | Descripción |
|---------|-------------|
| NAME_CONTRACT_TYPE | Tipo de contrato (cash, revolving) |
| CODE_GENDER | Género del cliente |
| FLAG_OWN_CAR | Posee automóvil (Y/N) |
| NAME_INCOME_TYPE | Tipo de ingreso |
| FLAG_OWN_REALTY | Posee propiedad (Y/N) |
| FAMILY_STATUS | Estado civil / familiar |
| OCCUPATION_TYPE | Tipo de ocupación |

**Temas cubiertos:**
- Carga con `pd.read_csv()` y `on_bad_lines='skip'`
- Exploración con `.head()`, `.describe()`, `.info()`
- Nulos con `.isnull().sum()`
- Distribución categórica con `.value_counts()`
- Histograma con línea de media usando `plt.axvline()`
- Boxplot por grupo familiar con Seaborn

**Código de ejemplo:**

```python
# Carga del dataset
data = pd.read_csv("/content/credit_card.csv", on_bad_lines='skip')

# Análisis de nulos
data.isnull().sum()

# Histograma con media
data['CREDIT'] = pd.to_numeric(data['CREDIT'], errors='coerce')
promedio = data['CREDIT'].mean()
plt.hist(data['CREDIT'], bins=10, color='blue', rwidth=0.7)
plt.axvline(promedio, color='red', linestyle='dashed', linewidth=2,
            label=f'Media: {promedio:.2f}')

# Boxplot Seaborn
sns.set_theme(style="ticks")
sns.boxplot(data=data, x='FAM_MEMBERS', y='CREDIT',
            palette="viridis",
            medianprops={"color": "yellow", "linewidth": 2})
sns.despine(offset=10, trim=True)
```

**Conceptos clave:**
- `pd.read_csv()` — carga de archivos CSV
- `on_bad_lines='skip'` — omitir filas con errores
- `pd.to_numeric(errors='coerce')` — conversión segura a número
- `plt.axvline()` — línea vertical de referencia en el gráfico
- `sns.boxplot()` — diagrama de caja con Seaborn
- `sns.despine()` — limpieza visual del gráfico

```bash
pip install pandas matplotlib seaborn
```

---

## 🟪 Clase 5 — Estadística Descriptiva y Visualización

**Archivo:** `clase_5.py` | **Nivel:** Avanzado | **Dataset:** Sintético (seed=42, 1000 empleados)

Análisis estadístico completo: tendencia central, dispersión, outliers y comparaciones por departamento.

**Estructura del dataset:**

| Columna | Distribución |
|---------|-------------|
| ID_Empleado | 1 al 1000 |
| Departamento | Ingeniería 50%, Ventas 30%, Marketing 15%, Directivos 5% |
| Edad | Normal (media=34, std=8) |
| Años_Experiencia | Normal (media=8, std=4), recortada entre 0 y 40 |
| Puntaje_desempeño | Normal (media=75, std=12), recortada entre 0 y 100 |
| Salario_USD | Normal (media=5000, std=2000), recortada entre 1000 y 30000 |

**Temas cubiertos:**
- `np.random.seed(42)` — reproducibilidad garantizada
- `plt.subplots(2, 2)` — grilla con barras, histograma, scatter y boxplot
- Outliers salariales — simulación de ejecutivos con salarios extremos
- Media vs Mediana — impacto visual de los outliers
- Regla de Tukey — `IQR = Q3 - Q1`, límites `±1.5 × IQR`
- Boxplots por departamento — comparativa de edad, salario y desempeño

**Código de ejemplo:**

```python
# Dataset sintético reproducible
np.random.seed(42)
n = 1000

df_hr = pd.DataFrame({
    'ID_Empleado': range(1, n+1),
    'Departamento': np.random.choice(
        ['Ingeniería', 'Ventas', 'Marketing', 'Directivos'],
        size=n, p=[0.50, 0.30, 0.15, 0.05]
    ),
    'Edad': np.random.normal(34, 8, n).clip(18, 65).astype(int),
    'Salario_USD': np.random.normal(5000, 2000, n).clip(1000, 30000).round(1)
})

# Detección de outliers con regla de Tukey
Q1 = df_hr['Edad'].quantile(0.25)
Q3 = df_hr['Edad'].quantile(0.75)
IQR = Q3 - Q1
lim_sup = Q3 + 1.5 * IQR
lim_inf = Q1 - 1.5 * IQR

# Media vs Mediana
media_salario   = df_hr['Salario_USD'].mean()
mediana_salario = df_hr['Salario_USD'].median()

sns.histplot(datos, kde=True)
plt.axvline(media_salario,   color='red',   linestyle='--', label='Media')
plt.axvline(mediana_salario, color='green', linestyle='-',  label='Mediana')
```

**Conceptos clave:**
- `np.random.seed()` — reproducibilidad de datos aleatorios
- `.clip(min, max)` — limitar valores a un rango específico
- `.quantile()` — cálculo de cuartiles Q1 y Q3
- IQR — rango intercuartílico como medida de dispersión
- Regla de Tukey — detección de outliers con 1.5 × IQR
- `sns.histplot(kde=True)` — histograma con curva de densidad suavizada

```bash
pip install pandas numpy matplotlib seaborn
```

---

## 📊 Proyectos y Evaluaciones

### trabajocustomers.py — Análisis de Clientes

Análisis completo del comportamiento de una base de clientes: limpieza, exploración estadística, segmentación y visualización de patrones.

- Gráficos avanzados para analizar la mediana y moda de ingresos por género
- Segmentación de clientes por perfil de comportamiento
- Pipeline completo: carga → limpieza → EDA → visualización → conclusiones

---

### parcial.py — Análisis de Crédito

Generación de dataset sintético con análisis de correlación entre variables socioeconómicas y aprobación de crédito.

- Variables: nivel educativo, salario, aprobación de crédito
- Análisis de correlación entre educación, ingreso y riesgo crediticio
- Histogramas, boxplots y detección de outliers

---

### poster.py — Visualización Resumen

Script para generar visualizaciones de resumen con los principales hallazgos del portafolio.

---

## 🛠️ Tecnologías Utilizadas

| Tecnología | Uso Principal |
|------------|---------------|
| Python 3 | Lenguaje principal de análisis |
| NumPy | Computación numérica y generación de datos |
| Pandas | Manipulación y análisis de datos tabulares |
| Matplotlib | Visualización básica y personalizada |
| Seaborn | Visualización estadística avanzada |
| Power BI | Dashboards interactivos de negocio |
| Jupyter Notebook | Análisis interactivo y exploración |

---

## ⚙️ Instalación

**1. Clonar el repositorio:**

```bash
git clone https://github.com/tu-usuario/portafolio-data-science.git
cd portafolio-data-science
```

**2. Instalar dependencias:**

```bash
pip install numpy pandas matplotlib seaborn pyarrow
```

**3. Ejecutar un script:**

```bash
python clase_1.py
```

> También puedes abrir los notebooks directamente en [Google Colab](https://colab.research.google.com/).

---

*Juan Pablo · Portafolio de Ciencia de Datos · Documentando el aprendizaje, un dataset a la vez.*