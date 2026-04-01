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
    NAME_INCOME_TYPE, FLAG_OWN_REALTY, FAMILY_STATUS

===================================================
  README - CLASE 5: ESTADÍSTICA DESCRIPTIVA Y
           VISUALIZACIÓN DE DATOS (RRHH)
====================================================

DESCRIPCIÓN GENERAL
-------------------
Este notebook (clase5.ipynb) trabaja con un dataset sintético de 1000
empleados generado con NumPy. Se aplican técnicas de estadística
descriptiva (media, mediana, cuartiles, IQR) y se visualizan con
Matplotlib y Seaborn para analizar edad, salario y desempeño.

----------------------------------------------------
SECCIONES DEL CÓDIGO
----------------------------------------------------

1. CONFIGURACIÓN INICIAL
   - Se importan las librerías principales:
       pandas, numpy, matplotlib.pyplot, seaborn
   
   - Se configura el estilo global de Seaborn:
       sns.set_theme(style='whitegrid', palette='deep')
       plt.rcParams['figure.figsize'] = (10, 8)

----------------------------------------------------

2. GENERACIÓN DEL DATASET SINTÉTICO
   - Se usa np.random.seed(42) para reproducibilidad. La semilla fija
     el generador pseudoaleatorio y garantiza los mismos resultados
     cada vez que se ejecuta el código.
   
   - Se crea un DataFrame con 1000 empleados y estas columnas:
   
       ID_Empleado       -> Número del 1 al 1000
       Departamento      -> Elegido aleatoriamente con probabilidades:
                            Ingeniería 50%, Ventas 30%, Marketing 15%, Directivos 5%
       Edad              -> Distribución normal: media=34, std=8
       Años_Experiencia  -> Normal: media=8, std=4, recortada entre 0 y 40
       Puntaje_desempeño -> Normal: media=75, std=12, recortada entre 0 y 100
   
   Métodos usados:
       np.random.choice()     -> Selección aleatoria con probabilidades (p=[...])
       np.random.normal()     -> Distribución normal (media, desviación estándar, n)
       .clip(min, max)        -> Recorta valores fuera del rango especificado
       .astype(int)           -> Convierte a entero
       .round(1)              -> Redondea a 1 decimal

----------------------------------------------------

3. VISUALIZACIONES INICIALES (GRILLA 2x2)
   - Se usa plt.subplots(2, 2) para crear 4 gráficas en un solo panel:
   
       [0,0] Barras         -> Empleados por departamento (value_counts + bar)
       [0,1] Histograma     -> Distribución de edad (20 bins, color coral)
       [1,0] Scatter        -> Experiencia vs Puntaje de desempeño (alpha=0.5)
       [1,1] Boxplot        -> Desempeño por departamento (df.boxplot)
   
   - plt.tight_layout() ajusta automáticamente el espaciado entre paneles.

----------------------------------------------------

4. VALORES ATÍPICOS EN SALARIO (OUTLIERS)
   - Se agregan salarios extremos a 5 directivos seleccionados al azar:
       outlier_idx = df_hr[df_hr['Departamento'] == 'Directivos'].sample(5).index
       df_hr.loc[outlier_idx, 'Salario_USD'] = [1500000, 2800000, 320000, 190000, 450000]
   
   - Esto simula una situación real donde altos ejecutivos distorsionan
     la media salarial del conjunto.
   
   - Se calcula y compara media vs mediana:
       media_salario    -> Afectada por los outliers (más alta)
       mediana_salario  -> Más representativa del empleado típico

----------------------------------------------------

5. DISTRIBUCIÓN DE SALARIOS: MEDIA VS MEDIANA
   - Se reconstruye el dataset completo con columna Salario_USD generada
     con distribución normal: media=5000, std=2000, recortada [1000, 30000]
   
   - Se filtra datos para el gráfico:
       datos = df_hr[df_hr['Salario_USD'] < 35000]
   
   - sns.histplot con kde=True agrega una curva de densidad suavizada
     sobre el histograma.
   
   - Se trazan dos líneas verticales:
       plt.axvline(media_salario,   color='red',   linestyle='--')
       plt.axvline(mediana_salario, color='green', linestyle='-')
   
   - La diferencia visual entre ambas líneas ilustra el efecto de los
     valores extremos sobre la media.

----------------------------------------------------

6. MEDIDAS DE TENDENCIA CENTRAL Y DISPERSIÓN (EDAD)
   - Se calculan los estadísticos clave de la columna Edad:
   
       Q1  = quantile(0.25)       -> Cuartil 1 (25% de los datos)
       Q3  = quantile(0.75)       -> Cuartil 3 (75% de los datos)
       IQR = Q3 - Q1              -> Rango intercuartílico
       lim_sup = Q3 + 1.5 * IQR  -> Límite superior para outliers
       lim_inf = Q1 - 1.5 * IQR  -> Límite inferior para outliers
   
   - Valores fuera de [lim_inf, lim_sup] se consideran atípicos (regla de Tukey).
   
   - El boxplot se complementa con líneas verticales que marcan:
       Q1, Q3, Mediana, Media, Límite superior e inferior

----------------------------------------------------

7. BOXPLOTS POR DEPARTAMENTO
   - Se generan tres boxplots comparativos usando sns.boxplot:
   
       Edad por Departamento
       -> figsize=(30,40), ylim=(0,70)
       -> Permite ver si hay diferencias de edad entre áreas
   
       Salario_USD por Departamento
       -> figsize=(30,40), ylim=(0,200000)
       -> El área Directivos mostrará outliers extremos
   
       Puntaje_desempeño por Departamento
       -> figsize=(12,6), paleta de colores por área
       -> Se agregan líneas horizontales con axhline() para la
          media y mediana globales como referencia de comparación

----------------------------------------------------

CONCEPTOS CLAVE APRENDIDOS
---------------------------
  * np.random.seed()         -> Reproducibilidad de datos aleatorios
  * np.random.normal()       -> Generación de distribución normal
  * .clip()                  -> Limitar valores a un rango
  * .quantile()              -> Cálculo de cuartiles
  * IQR                      -> Rango intercuartílico (dispersión)
  * Regla de Tukey           -> Detección de outliers con 1.5 * IQR
  * Media vs Mediana         -> Efecto de outliers en cada medida
  * sns.histplot(kde=True)   -> Histograma con curva de densidad
  * plt.axvline/axhline()    -> Líneas de referencia en gráficos
  * sns.boxplot()            -> Diagrama de caja por grupos
  * plt.subplots(2, 2)       -> Grilla de múltiples gráficas

----------------------------------------------------

DEPENDENCIAS REQUERIDAS
-----------------------
  - Python 3.x
  - pandas
  - numpy
  - matplotlib
  - seaborn

----------------------------------------------------

DATASET UTILIZADO
-----------------
  - Dataset sintético generado en el mismo notebook con seed=42
  - 1000 empleados, columnas: ID_Empleado, Departamento, Edad,
    Años_Experiencia, Puntaje_desempeño, Salario_USD