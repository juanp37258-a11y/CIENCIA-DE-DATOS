8# 📊 Mi Proyecto de Data Science

## 📁 Estructura de archivos

| Archivo | Descripción |
|--------|-------------|
| `clase_1.py` | Clase 1 |
| `clase_2.py` | Clase 2 |
| `clase3.py` | Clase 3 |
| `clase4.py` | Clase 4 |
| `clase5.py` | Clase 5 |
| `trabajocustomers.py` | Análisis de clientes |
| `poster.jpeg` | Imagen del proyecto |
| `powe bi.png` | Dashboard Power BI |



## 📘 clase_1.py

Primer acercamiento a las librerías fundamentales de Data Science.

### Temas:
- **NumPy** — arrays, matrices, operaciones matemáticas
- **Juego de dados** — números aleatorios con `np.random`
- **Juego de cartas** — arrays 2D
- **Matplotlib** — gráficas de líneas y vectores
- **Pandas** — Series, DataFrames, `df.head()`

### Actividad:
```python
# NumPy - operaciones básicas
import numpy as np
multiplicacion = np.array(2*3)
eye_range = np.eye(7)
division = np.array(7/2)

# Juego de dados
dado = np.random.randint(low=1, high=7)

# Juego de cartas
all_cards = np.array([pikas, trebol, diamante, corazon])

# Matplotlib - gráfica de crecimiento
plt.plot(edad, crecimiento, marker='o', linestyle='-')
plt.title('Growth Over Time with Random Variation')

# Pandas - DataFrame de productos
new_df = pd.DataFrame({"producto": [...], "precio": [...], "cantidad": [...]})
new_df.head()
```


## 📗 clase_2.py

Introducción profunda a Pandas: Series, DataFrames y exportación de datos.

### Temas:
- **Series** — creación con índices personalizados
- **DataFrame** — filtros, selección de columnas, `loc` e `iloc`
- **Matplotlib** — gráfica de Series
- **Exportación** — `.csv`, `.html`, `.json`

### Actividad:
```python
# Series con índice
s = pd.Series([2, 4, 6, 8], index=["num1", "num2", "num3", "num4"])

# DataFrame de personas
personas = {
    "peso": pd.Series([84, 90, 56, 64], ["Santiago","Pedro","Ana","Julia"]),
    "altura": pd.Series({"Santiago": 187, "Pedro": 178, "Julia": 170, "Ana": 165}),
    "hijos": pd.Series([2, 3], ["Pedro", "Julia"])
}
df = pd.DataFrame(personas)

# Filtros
df[df["peso"] > 80]
df.loc["Ana"]
df.iloc[1:3]

# Exportar
df.to_csv("df_personas.csv")
df.to_html("df_personas.html")
df.to_json("df_personas.json")

```
📊 Clase 3 — Introducción a Matplotlib
Notebook generado en Google Colab como parte del curso de Ciencia de Datos.
Cubre los fundamentos de visualización de datos con la librería matplotlib.
📚 Contenido
1. Instalación e importación
!pip install matplotlib
import matplotlib
import matplotlib.pyplot as plt
import numpy as np
2. Gráfico de línea básico
Se grafica una lista de valores simples con plt.plot().
plt.plot([1, 2, 5, 3, 4, 5, 1])

📚 Temas:
📂 Carga de datos — lectura de CSV real con pd.read_csv()
🔍 Exploración — head(), describe(), info(), isnull().sum()
📊 Conteo de categorías — value_counts() en género, contrato, ocupación, estado civil
📈 Histograma — distribución del monto de crédito con línea de media
📦 Boxplot con Seaborn — crédito por miembros de la familia con paleta viridis


📊 clase4.py
Análisis exploratorio y visualización de datos reales de crédito bancario con Pandas, Matplotlib y Seaborn.

🎯 Objetivos
Cargar y explorar un dataset real de solicitudes de crédito bancario
Identificar valores nulos y distribución de variables categóricas
Visualizar la distribución del monto de crédito con histograma y media
Analizar el crédito según los miembros del hogar mediante un boxplot

🗂️ Dataset — credit_card.csv
Columna
Descripción
NAME_CONTRACT_TYPE
Tipo de contrato
CODE_GENDER
Género del cliente
FLAG_OWN_CAR
Tiene auto propio
FLAG_OWN_REALTY
Tiene propiedad
NAME_INCOME_TYPE
Tipo de ingreso
FAMILY_STATUS
Estado civil
OCCUPATION_TYPE
Tipo de ocupación
FAM_MEMBERS
Miembros de la familia
CREDIT
Monto del crédito



