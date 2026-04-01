7# 📊 Mi Portafolio de Ciencia de Datos

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




## 🟩 clase_1.py

Fundamentos de Data Science con Python: arrays, simulaciones y visualización de datos.

### 📖 Temas

- **NumPy** — creación de arrays, matrices y operaciones con `np.array`, `np.eye`
- **Aleatoriedad** — generación de números con `np.random.rand` y `np.random.randint`
- **Juego de Dados** — simulación de tiradas con resultados enteros
- **Juego de Cartas** — representación de mazos con arrays 2D
- **Matplotlib** — graficación de vectores, matrices y curvas con variación aleatoria
- **Pandas** — primeros pasos con `Series`, `DataFrame` y datos de estatura

### 🎲 Simulación de dado

```python
dado = np.random.randint(low=1, high=7)
```

### 🃏 Mazo de cartas

```python
all_cards = np.array([pikas, trebol, diamante, corazon])
```

### 📈 Curva de crecimiento

```python
crecimiento = edad * 6 + np.random.randn(len(edad)) * 2
plt.plot(edad, crecimiento, marker='o')
plt.show()
```

### 🗂️ DataFrame de estatura

```python
datos_estatura = {
    "nombre": ["luis", "paco", "augusto"],
    "apellido": ["gonzales", "rojas", "lopez"],
    "edad": [23, 34, 2],
    "estatura": [1.60, 1.69, 1.87]
}
df = pd.DataFrame(datos_estatura)
```

### ⚙️ Requisitos

```bash
pip install numpy matplotlib pandas

# 🟦 clase_2.py

Introducción profunda a Pandas: Series, DataFrames y manipulación de datos tabulares.

### 📖 Temas

- **Pandas** — instalación y configuración con `pyarrow`
- **Series** — creación con índices y valores personalizados
- **DataFrame** — estructuras de datos tabulares con múltiples columnas
- **Manipulación** — filtros, selección de columnas con `loc` e `iloc`
- **Exportación** — guardado de datos en `.csv`, `.html`, `.json`

### 📊 Serie básica de Pandas

```python
s = pd.Series([2, 4, 6, 8, 10])
```

### 🗂️ DataFrame básico

```python
df = pd.DataFrame({'A': [1, 2, 3], 'B': [4, 5, 6], 'C': [2, 3, 4]})
```

### ⚙️ Requisitos

```bash
pip install pandas pyarrow

README - CLASE 3: INTRODUCCIÓN A MATPLOTLIB
====================================================

DESCRIPCIÓN GENERAL
-------------------
Este notebook (clase3.ipynb) es una introducción práctica a la librería
Matplotlib en Python, ejecutada en Google Colab. Cubre la creación de
distintos tipos de gráficas: líneas, dispersión e histogramas.

----------------------------------------------------
SECCIONES DEL CÓDIGO
----------------------------------------------------

1. INSTALACIÓN E IMPORTACIÓN
   - Se instala e importa matplotlib:
       pip install matplotlib
       import matplotlib.pyplot as plt
   - También se usa numpy para generar datos:
       import numpy as np

----------------------------------------------------

2. GRÁFICA DE LÍNEA BÁSICA
   - Se grafica una lista simple de valores:
       plt.plot([1, 2, 5, 3, 4, 5, 1])
       plt.show()
   - Matplotlib conecta los puntos en orden automáticamente.

----------------------------------------------------

3. GRÁFICA CON NUMPY (PARÁBOLA)
   - Se generan 500 puntos entre 0 y 3 con np.linspace:
       x = np.linspace(3, 0, 500)
       y = x**2
       plt.plot(x, y)
   - np.linspace crea un arreglo de valores igualmente espaciados.

----------------------------------------------------

4. MÚLTIPLES LÍNEAS, LEYENDA Y GRILLA
   - Se grafican dos funciones en el mismo plot:
       plt.plot(x, x**2, 'b--', label="x²")   -> azul, línea punteada
       plt.plot(x, x+1,  'g',   label="x+1")  -> verde, línea sólida
       plt.legend()   -> muestra la leyenda
       plt.grid()     -> activa la cuadrícula

----------------------------------------------------

5. SUBPLOTS (MÚLTIPLES PANELES)
   - Se crean dos gráficas lado a lado con plt.subplots:
       fig, ax = plt.subplots(1, 2, figsize=(14, 6))
       ax[0].plot(x, y, 'r-', linewidth=3)       -> panel izquierdo
       ax[1].plot(x, y2, 'm--', linewidth=3)     -> panel derecho
   - Cada panel tiene su propio título y grilla con transparencia:
       ax[0].set_title("Parábola", fontsize=16)
       ax[0].grid(alpha=0.3)

----------------------------------------------------

6. GRÁFICA DE DISPERSIÓN (SCATTER)
   - Se generan puntos aleatorios con numpy:
       x, y = rand(2, 10)
       plt.scatter(x, y)
   - Scatter muestra puntos individuales sin conectarlos.
   
   - Versión con dos grupos de 100 puntos y colores distintos:
       x, y   = rand(2, 100)  -> grupo azul
       x2, y2 = rand(2, 100)  -> grupo verde
       plt.scatter(x, y, c='blue')
       plt.scatter(x2, y2, c='green')

----------------------------------------------------

7. HISTOGRAMAS
   - Un histograma muestra la distribución de frecuencias de los datos.
   
   Primer ejemplo con bins automáticos y personalizados:
       data = [1, 1.3, 1.5, 2, 2, 0.2, 3, 3, 3, 3]
       ax1.hist(data, bins=10, ...)              -> 10 intervalos automáticos
       ax2.hist(data, bins=[1, 3, 3, 2.5, 3], ...)  -> intervalos manuales
   
   Segundo ejemplo más limpio:
       data = [2, 2.3, 2.8, 3, 3.5, 4.1, 4, 4, 5, 5.2, 5.8, 6]
       ax1.hist(data, bins=8, ...)               -> 8 bins automáticos
       ax2.hist(data, bins=[2, 3, 4, 5, 6], ...) -> bins manuales exactos
   
   Parámetros usados:
       bins      -> cantidad o bordes de los intervalos
       rwidth    -> ancho relativo de las barras (0 a 1)
       color     -> color de relleno
       edgecolor -> color del borde de las barras

----------------------------------------------------

8. GUARDAR GRÁFICA EN ARCHIVO
   - Se guarda la gráfica como imagen PNG:
       fig.savefig("mi_grafica.png", transparent=True)
   - transparent=True hace que el fondo sea transparente.

----------------------------------------------------

CONCEPTOS CLAVE APRENDIDOS
---------------------------
  * plt.plot()        -> Gráfica de línea
  * plt.scatter()     -> Gráfica de dispersión
  * plt.hist()        -> Histograma
  * plt.legend()      -> Leyenda de series
  * plt.grid()        -> Cuadrícula de fondo
  * plt.subplots()    -> Múltiples paneles en una figura
  * ax.set_title()    -> Título de un panel
  * ax.set_xlabel/ylabel() -> Etiquetas de ejes
  * plt.tight_layout() -> Ajuste automático de espaciado
  * fig.savefig()     -> Guardar figura como archivo

----------------------------------------------------

DEPENDENCIAS REQUERIDAS
-----------------------
  - Python 3.x
  - matplotlib
  - numpy

```
README - CLASE 4: ANÁLISIS EXPLORATORIO DE DATOS
====================================================

DESCRIPCIÓN GENERAL
-------------------
Este notebook (clase4.ipynb) trabaja con un dataset real de tarjetas de
crédito (credit_card.csv) y aplica técnicas de exploración, limpieza y
visualización de datos usando Pandas, Matplotlib y Seaborn.

----------------------------------------------------
SECCIONES DEL CÓDIGO
----------------------------------------------------

1. CARGA DEL DATASET
   - Se carga un archivo CSV con datos de clientes de crédito:
       data = pd.read_csv("/content/credit_card.csv", on_bad_lines='skip')
   - on_bad_lines='skip' ignora filas con errores de formato en lugar
     de detener la ejecución.

----------------------------------------------------

2. EXPLORACIÓN INICIAL DEL DATAFRAME
   
   data.head()
   -> Muestra las primeras 5 filas del dataset.
   
   data.describe()
   -> Estadísticas descriptivas de columnas numéricas:
      count, mean, std, min, max, percentiles 25/50/75.
   
   data.info()
   -> Resumen del DataFrame: tipos de datos, cantidad de valores
      no nulos y uso de memoria.
   
   data['NAME_CONTRACT_TYPE'].info()
   -> Información específica de una sola columna.

----------------------------------------------------

3. ANÁLISIS DE VALORES NULOS
   
   data.isnull()
   -> Tabla de True/False indicando dónde hay valores nulos.
   
   data.isnull().sum()
   -> Cuenta los valores nulos por columna — útil para decidir
      qué columnas necesitan limpieza.

----------------------------------------------------

4. CONTEO DE VALORES CATEGÓRICOS (value_counts)
   - Se analiza la distribución de las siguientes columnas:
   
       NAME_CONTRACT_TYPE  -> Tipo de contrato (ej: cash, revolving)
       CODE_GENDER         -> Género del cliente
       FLAG_OWN_CAR        -> Si posee automóvil (Y/N)
       NAME_INCOME_TYPE    -> Tipo de ingreso (empleado, pensionado, etc.)
       FLAG_OWN_REALTY     -> Si posee propiedad (Y/N)
       FAMILY_STATUS       -> Estado civil / familiar
       OCCUPATION_TYPE     -> Tipo de ocupación
   
   - value_counts() devuelve cuántas veces aparece cada valor único,
     ordenado de mayor a menor frecuencia.

----------------------------------------------------

5. HISTOGRAMA DE CRÉDITO CON LÍNEA DE MEDIA
   
   - Se convierte la columna CREDIT a numérico:
       data['CREDIT'] = pd.to_numeric(data['CREDIT'], errors='coerce')
     * errors='coerce' convierte valores no numéricos en NaN.
   
   - Se grafica la distribución del monto de crédito:
       plt.hist(data['CREDIT'], bins=10, color='blue', rwidth=0.7)
   
   - Se calcula y traza la línea de la media:
       promedio = data['CREDIT'].mean()
       plt.axvline(promedio, color='red', linestyle='dashed', linewidth=2,
                   label=f'Media: {promedio:.2f}')
   
   - plt.axvline() dibuja una línea vertical en el valor indicado.
   - f'Media: {promedio:.2f}' formatea el número con 2 decimales.
   - plt.xticks(rotation=40) rota las etiquetas del eje X para legibilidad.

----------------------------------------------------

6. BOXPLOT CON SEABORN
   - Se visualiza la distribución del crédito agrupada por cantidad
     de miembros familiares.
   
   Configuración:
       sns.set_theme(style="ticks")   -> Estilo de fondo con marcas
       plt.figure(figsize=(12, 6))    -> Tamaño del lienzo
   
   Boxplot:
       sns.boxplot(
           data=data,
           x='FAM_MEMBERS',    -> Eje X: grupos por miembros familiares
           y='CREDIT',         -> Eje Y: monto del crédito
           hue='FAM_MEMBERS',  -> Color distinto por grupo
           palette="viridis",  -> Paleta de colores
           legend=False,       -> Oculta la leyenda (redundante con hue)
           medianprops={"color": "yellow", "linewidth": 2}  -> Mediana amarilla
       )
   
   - Un boxplot muestra: mínimo, Q1, mediana, Q3, máximo y valores atípicos.
   
   Ajustes finales:
       sns.despine(offset=10, trim=True) -> Elimina bordes del gráfico
       plt.ticklabel_format(style='plain', axis='y')
       -> Evita notación científica en el eje Y (ej: 1000000 en lugar de 1e6)

----------------------------------------------------

CONCEPTOS CLAVE APRENDIDOS
---------------------------
  * pd.read_csv()           -> Carga de archivos CSV
  * on_bad_lines='skip'     -> Omitir filas con errores
  * .head()                 -> Vista previa del dataset
  * .describe()             -> Estadísticas descriptivas
  * .info()                 -> Tipos y nulos por columna
  * .isnull().sum()         -> Conteo de valores nulos
  * .value_counts()         -> Frecuencia de valores categóricos
  * pd.to_numeric(errors='coerce') -> Conversión segura a número
  * plt.axvline()           -> Línea vertical en gráfico
  * sns.boxplot()           -> Diagrama de caja con Seaborn
  * sns.despine()           -> Limpieza visual del gráfico
  * ticklabel_format()      -> Formato de etiquetas numéricas

----------------------------------------------------

DEPENDENCIAS REQUERIDAS
-----------------------
  - Python 3.x
  - pandas
  - matplotlib
  - seaborn

----------------------------------------------------

DATASET UTILIZADO
-----------------
  - Archivo: credit_card.csv
  - Columnas relevantes: NAME_CONTRACT_TYPE, CODE_GENDER, FLAG_OWN_CAR,
    NAME_INCOME_TYPE, FLAG_OWN_REALTY, FAMILY_STATUS, OCCUPATION_TYPE,
    CREDIT, FAM_MEMBERS

====================================================
  Archivo generado como documentación del notebook
  clase4.ipynb - Análisis Exploratorio de Datos
============================================