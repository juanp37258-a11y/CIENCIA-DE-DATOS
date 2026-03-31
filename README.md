# 📊 Mi Proyecto de Data Science

## 📁 Estructura de archivos

| Archivo | Descripción |
|--------|-------------|
| `clase_1.py` | Clase 1 |
| `clase_2.py` | Clase 2 |
| `clase_3.py` | Clase 3 |
| `clase_4.py` | Clase 4 |
| `clase_5.py` | Clase 5 |
| `trabajocustomers.py` | Análisis de clientes |
| `poster.jpeg` | Imagen del proyecto |
| `power_bi.png` | Dashboard Power BI |


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

## 📊 clase_3.py

Introducción a Matplotlib: Visualización de datos con gráficos.

### Temas:
- **Instalación e importación** — setup de matplotlib y librerías necesarias
- **Gráficos de línea** — `plt.plot()` y personalización
- **Carga de datos** — lectura de CSV real con `pd.read_csv()`
- **Exploración de datos** — `head()`, `describe()`, `info()`, `isnull().sum()`
- **Conteo de categorías** — `value_counts()` en género, contrato, ocupación, estado civil
- **Histograma** — distribución del monto de crédito con línea de media
- **Boxplot con Seaborn** — crédito por miembros de la familia con paleta viridis

### Actividad:
```python
import matplotlib.pyplot as plt
import matplotlib
import numpy as np
import pandas as pd

# Gráfico de línea básico
plt.plot([1, 2, 5, 3, 4, 5, 1])
plt.title('Gráfico de Línea Básico')
plt.show()

# Cargar datos
df = pd.read_csv('credit_card.csv')

# Exploración
print(df.head())
print(df.describe())
print(df.info())
print(df.isnull().sum())

# Conteo de categorías
print(df['CODE_GENDER'].value_counts())
print(df['NAME_CONTRACT_TYPE'].value_counts())

# Histograma con media
plt.figure(figsize=(10, 6))
plt.hist(df['CREDIT'], bins=50, edgecolor='black')
plt.axvline(df['CREDIT'].mean(), color='red', linestyle='--', label=f'Media: {df["CREDIT"].mean():.0f}')
plt.title('Distribución del Monto de Crédito')
plt.xlabel('Monto')
plt.ylabel('Frecuencia')
plt.legend()
plt.show()
``` 

## 📙 clase_4.py

Análisis exploratorio y visualización avanzada de datos reales de crédito bancario.

### Temas:
- **Carga y exploración** — dataset real de solicitudes de crédito bancario
- **Manejo de valores nulos** — identificación y tratamiento
- **Distribución de variables categóricas** — análisis de género, contrato, ocupación, estado civil
- **Visualización con Histograma** — distribución del monto de crédito con línea de media
- **Boxplot con Seaborn** — análisis de crédito según miembros del hogar
- **Paletas de color** — uso de viridis y otras paletas

### Dataset — credit_card.csv

| Columna | Descripción |
|---------|-------------|
| `NAME_CONTRACT_TYPE` | Tipo de contrato |
| `CODE_GENDER` | Género del cliente |
| `FLAG_OWN_CAR` | Tiene auto propio |
| `FLAG_OWN_REALTY` | Tiene propiedad |
| `NAME_INCOME_TYPE` | Tipo de ingreso |
| `FAMILY_STATUS` | Estado civil |
| `OCCUPATION_TYPE` | Tipo de ocupación |
| `FAM_MEMBERS` | Miembros de la familia |
| `CREDIT` | Monto del crédito |

### Actividad:
```python
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns

# Cargar datos
df = pd.read_csv('credit_card.csv')

# Exploración básica
print(f"Shape: {df.shape}")
print(f"Valores nulos:\n{df.isnull().sum()}")
print(f"\nInfo:\n{df.info()}")

# Análisis de variables categóricas
print(f"\nGénero:\n{df['CODE_GENDER'].value_counts()}")
print(f"\nTipo de Contrato:\n{df['NAME_CONTRACT_TYPE'].value_counts()}")
print(f"\nEstado Civil:\n{df['FAMILY_STATUS'].value_counts()}")
print(f"\nOcupación:\n{df['OCCUPATION_TYPE'].value_counts()}")

# Histograma del monto de crédito
plt.figure(figsize=(10, 6))
plt.hist(df['CREDIT'], bins=50, edgecolor='black', alpha=0.7)
plt.axvline(df['CREDIT'].mean(), color='red', linestyle='--', linewidth=2, label=f'Media: {df["CREDIT"].mean():.0f}')
plt.title('Distribución del Monto de Crédito')
plt.xlabel('Monto ($)')
plt.ylabel('Frecuencia')
plt.legend()
plt.show()

# Boxplot: Crédito por miembros de la familia
plt.figure(figsize=(10, 6))
sns.boxplot(data=df, x='FAM_MEMBERS', y='CREDIT', palette='viridis')
plt.title('Distribución del Crédito por Miembros de la Familia')
plt.xlabel('Miembros de la Familia')
plt.ylabel('Monto del Crédito ($)')
plt.show()
```