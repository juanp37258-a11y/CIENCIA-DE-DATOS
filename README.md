# 📊 Mi Proyecto de Data Science

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

---
