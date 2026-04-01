�

📊 Portafolio de Ciencia de Datos
Juan Pablo | Data Science Portfolio

Colección progresiva de proyectos, scripts educativos y recursos profesionales en Ciencia de Datos, Análisis de Información y Visualización.
�

🧭 Tabla de Contenidos
Introducción
Estructura del Repositorio
Clases Prácticas
Clase 1 — NumPy, Pandas y Matplotlib
Clase 2 — Pandas Avanzado
Clase 3 — Matplotlib
Clase 4 — EDA con Dataset Real
Clase 5 — Estadística Descriptiva
Proyectos y Evaluaciones
Recursos Visuales
Tecnologías Utilizadas
Instalación
📌 Introducción
Este repositorio documenta mi trayecto de aprendizaje en Ciencia de Datos, desde conceptos fundamentales de Python hasta análisis complejos sobre datasets reales. El portafolio está organizado en tres pilares:
Pilar
Descripción
🎓 Formación Académica
Series de lecciones progresivas en Python aplicadas a ciencia de datos
🔬 Proyectos Prácticos
Casos reales con limpieza, exploración y segmentación de datos
📢 Visualización y Comunicación
Dashboards e informes que comunican resultados efectivamente
El énfasis está en la interpretación de resultados y la comunicación de insights, no solo en el código.
📁 Estructura del Repositorio
📦 portafolio-data-science/
├── 📂 clases/
│   ├── clase_1.py          # NumPy, Pandas y Matplotlib básico
│   ├── clase_2.py          # Pandas avanzado y exportación de datos
│   ├── clase_3.py          # Visualización con Matplotlib
│   ├── clase_4.py          # EDA con dataset real de crédito
│   └── clase_5.py          # Estadística descriptiva avanzada
├── 📂 proyectos/
│   ├── trabajocustomers.py # Análisis de comportamiento de clientes
│   ├── parcial.py          # Dataset sintético y análisis de crédito
│   └── poster.py           # Generador de visualizaciones resumen
├── 📂 recursos/
│   ├── poster.jpeg         # Imagen resumen con hallazgos clave
│   └── power_bi.png        # Dashboard interactivo en Power BI
└── README.md
📚 Clases Prácticas
🟩 Clase 1 — NumPy, Pandas y Matplotlib Básico
Archivo: clase_1.py | Nivel: Fundamentos
Introducción a los pilares del ecosistema de datos en Python: arrays multidimensionales, estructuras tabulares y graficación básica.
Temas cubiertos:
NumPy — creación de arrays, matrices (np.array, np.eye) y operaciones elementales
Aleatoriedad — generación de números con np.random.rand y np.random.randint
Simulaciones — Juego de dados y mazo de cartas con arrays 2D
Matplotlib — graficación de vectores, matrices y curvas con variación aleatoria
Pandas — primeros pasos con Series, DataFrame y datos de estatura
Ejemplos de código:
# Simulación de dado
dado = np.random.randint(low=1, high=7)

# Mazo de cartas con arrays
all_cards = np.array([pikas, trebol, diamante, corazon])

# Curva de crecimiento con ruido aleatorio
crecimiento = edad * 6 + np.random.randn(len(edad)) * 2
plt.plot(edad, crecimiento, marker='o')
plt.show()

# DataFrame de estatura
datos_estatura = {
    "nombre": ["luis", "paco", "augusto"],
    "apellido": ["gonzales", "rojas", "lopez"],
    "edad": [23, 34, 2],
    "estatura": [1.60, 1.69, 1.87]
}
df = pd.DataFrame(datos_estatura)
pip install numpy matplotlib pandas
🟦 Clase 2 — Pandas Avanzado
Archivo: clase_2.py | Nivel: Intermedio
Manipulación profunda de datos tabulares con Pandas: filtros, selección y exportación en múltiples formatos.
Temas cubiertos:
Series — creación con índices y valores personalizados
DataFrame — estructuras tabulares con múltiples columnas y cálculos estadísticos
Filtros — selección avanzada con loc e iloc
Exportación — guardado de datos en .csv, .html, .json
Integración con pyarrow — backend optimizado para Pandas
Ejemplos de código:
# Serie básica
s = pd.Series([2, 4, 6, 8, 10])

# DataFrame con múltiples columnas
df = pd.DataFrame({'A': [1, 2, 3], 'B': [4, 5, 6], 'C': [2, 3, 4]})

# Exportación de datos
df.to_csv("datos.csv")
df.to_html("datos.html")
df.to_json("datos.json")
pip install pandas pyarrow
🟨 Clase 3 — Visualización con Matplotlib
Archivo: clase_3.py | Nivel: Intermedio
Creación de visualizaciones desde cero con Matplotlib, cubriendo los tipos de gráfico más utilizados en ciencia de datos.
Temas cubiertos:
Sección
Descripción
Gráfica de línea
Trazado de secuencias y curvas matemáticas
Parábola con NumPy
np.linspace para generar 500 puntos suaves
Múltiples líneas
Leyendas, grillas y estilos de línea
Subplots
Paneles múltiples con plt.subplots(1, 2)
Scatter
Gráficas de dispersión con grupos de colores
Histogramas
bins automáticos y manuales con rwidth
Guardar imagen
fig.savefig() con fondo transparente
Ejemplos de código:
# Múltiples líneas con leyenda
plt.plot(x, x**2, 'b--', label="x²")
plt.plot(x, x+1, 'g', label="x+1")
plt.legend()
plt.grid()

# Subplots lado a lado
fig, ax = plt.subplots(1, 2, figsize=(14, 6))
ax[0].plot(x, y, 'r-', linewidth=3)
ax[0].set_title("Parábola", fontsize=16)
ax[0].grid(alpha=0.3)

# Guardar con fondo transparente
fig.savefig("mi_grafica.png", transparent=True)
pip install matplotlib numpy
🟥 Clase 4 — Análisis Exploratorio (EDA)
Archivo: clase_4.py | Nivel: Intermedio-Avanzado | Dataset: credit_card.csv
Exploración, limpieza y visualización de un dataset real de tarjetas de crédito con Pandas, Matplotlib y Seaborn.
Temas cubiertos:
Carga de datos — pd.read_csv() con on_bad_lines='skip' para manejo de errores
Exploración inicial — .head(), .describe(), .info()
Valores nulos — .isnull().sum() para diagnóstico de calidad de datos
Variables categóricas — .value_counts() sobre columnas como género, tipo de contrato, ocupación
Histograma de crédito — distribución con línea de media usando plt.axvline()
Boxplot con Seaborn — distribución del crédito por número de miembros familiares
Dataset — columnas relevantes:
NAME_CONTRACT_TYPE  →  Tipo de contrato (cash, revolving)
CODE_GENDER         →  Género del cliente
FLAG_OWN_CAR        →  Posee automóvil (Y/N)
NAME_INCOME_TYPE    →  Tipo de ingreso
FLAG_OWN_REALTY     →  Posee propiedad (Y/N)
FAMILY_STATUS       →  Estado civil / familiar
OCCUPATION_TYPE     →  Tipo de ocupación
Ejemplos de código:
# Carga del dataset
data = pd.read_csv("/content/credit_card.csv", on_bad_lines='skip')

# Análisis de nulos
data.isnull().sum()

# Histograma con línea de media
data['CREDIT'] = pd.to_numeric(data['CREDIT'], errors='coerce')
promedio = data['CREDIT'].mean()
plt.hist(data['CREDIT'], bins=10, color='blue', rwidth=0.7)
plt.axvline(promedio, color='red', linestyle='dashed', linewidth=2,
            label=f'Media: {promedio:.2f}')

# Boxplot con Seaborn
sns.set_theme(style="ticks")
sns.boxplot(data=data, x='FAM_MEMBERS', y='CREDIT', hue='FAM_MEMBERS',
            palette="viridis", medianprops={"color": "yellow", "linewidth": 2})
sns.despine(offset=10, trim=True)
Conceptos clave:
pd.read_csv()              →  Carga de archivos CSV
on_bad_lines='skip'        →  Omitir filas con errores
pd.to_numeric(errors='coerce') →  Conversión segura a número
plt.axvline()              →  Línea vertical de referencia
sns.boxplot()              →  Diagrama de caja con Seaborn
sns.despine()              →  Limpieza visual del gráfico
ticklabel_format()         →  Formato de etiquetas numéricas
pip install pandas matplotlib seaborn
🟪 Clase 5 — Estadística Descriptiva y Visualización
Archivo: clase_5.py | Nivel: Avanzado | Dataset: Sintético (seed=42, 1000 empleados)
Análisis estadístico completo sobre un dataset sintético de empleados: medidas de tendencia central, dispersión, detección de outliers y comparaciones por grupo.
Estructura del dataset generado:
Columna
Descripción
Distribución
ID_Empleado
Identificador único
1 al 1000
Departamento
Área de trabajo
Ingeniería 50%, Ventas 30%, Marketing 15%, Directivos 5%
Edad
Edad del empleado
Normal (μ=34, σ=8)
Años_Experiencia
Años en industria
Normal (μ=8, σ=4), recortada [0, 40]
Puntaje_desempeño
Score de rendimiento
Normal (μ=75, σ=12), recortada [0, 100]
Salario_USD
Salario mensual
Normal (μ=5000, σ=2000), recortada [1000, 30000]
Temas cubiertos:
Reproducibilidad — np.random.seed(42) para resultados consistentes
Grilla de visualizaciones — plt.subplots(2, 2) con barras, histograma, scatter y boxplot
Outliers salariales — simulación de ejecutivos con salarios extremos ([150k, 280k, 32k...])
Media vs Mediana — impacto visual de outliers con plt.axvline() en ambas métricas
Regla de Tukey — detección de valores atípicos con IQR = Q3 - Q1 y límites ±1.5×IQR
Boxplots por departamento — comparación de Edad, Salario y Desempeño entre áreas
Ejemplos de código:
# Generación del dataset sintético reproducible
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

# Cálculo de estadísticos y detección de outliers
Q1 = df_hr['Edad'].quantile(0.25)
Q3 = df_hr['Edad'].quantile(0.75)
IQR = Q3 - Q1
lim_sup = Q3 + 1.5 * IQR
lim_inf = Q1 - 1.5 * IQR

# Comparación media vs mediana (efecto de outliers)
media_salario   = df_hr['Salario_USD'].mean()
mediana_salario = df_hr['Salario_USD'].median()

sns.histplot(datos, kde=True)
plt.axvline(media_salario,   color='red',   linestyle='--', label='Media')
plt.axvline(mediana_salario, color='green', linestyle='-',  label='Mediana')
Conceptos clave:
np.random.seed()        →  Reproducibilidad de datos aleatorios
.clip(min, max)         →  Limitar valores a un rango específico
.quantile()             →  Cálculo de cuartiles Q1, Q3
IQR                     →  Rango intercuartílico (medida de dispersión)
Regla de Tukey          →  Detección de outliers con 1.5 × IQR
Media vs Mediana        →  Efecto de outliers extremos en cada medida
sns.histplot(kde=True)  →  Histograma con curva de densidad suavizada
plt.axvline/axhline()   →  Líneas de referencia en gráficos
plt.subplots(2, 2)      →  Grilla de múltiples gráficas
pip install pandas numpy matplotlib seaborn
📊 Proyectos y Evaluaciones
🧑‍💼 trabajocustomers.py — Análisis de Clientes
Análisis completo del comportamiento de una base de clientes: limpieza de datos, exploración estadística, segmentación y visualización de patrones.
Highlights:
Gráficos avanzados para analizar la mediana y moda de ingresos por género
Segmentación de clientes por perfil de comportamiento
Pipeline completo: carga → limpieza → EDA → visualización → conclusiones
🏦 parcial.py — Análisis de Crédito
Generación de un dataset sintético de clientes con análisis de correlación entre variables socioeconómicas y aprobación de crédito.
Highlights:
Dataset sintético con variables: nivel educativo, salario, aprobación de crédito
Análisis de correlación entre educación, ingreso y riesgo crediticio
Visualizaciones: histogramas, boxplots, detección de outliers y tendencias
Conclusiones aplicables a decisiones de negocio
🎨 poster.py — Visualización Resumen
Script para generar visualizaciones de resumen y posters informativos con los principales hallazgos del portafolio.
🖼️ Recursos Visuales
Archivo
Descripción
poster.jpeg
Imagen resumen del proyecto con resultados, gráficos y hallazgos clave
power_bi.png
Dashboard interactivo con KPIs, métricas de negocio y análisis visual
🛠️ Tecnologías Utilizadas
Tecnología
Uso Principal
Python 3
Lenguaje principal de análisis
NumPy
Computación numérica y generación de datos
Pandas
Manipulación y análisis de datos tabulares
Matplotlib
Visualización básica y personalizada
Seaborn
Visualización estadística avanzada
Power BI
Dashboards interactivos de negocio
Jupyter Notebook
Análisis interactivo y exploración
⚙️ Instalación
1. Clonar el repositorio:
git clone https://github.com/tu-usuario/portafolio-data-science.git
cd portafolio-data-science
2. Instalar todas las dependencias:
pip install numpy pandas matplotlib seaborn pyarrow
3. Ejecutar cualquier script:
python clase_1.py
También puedes abrir los notebooks .ipynb directamente en Google Colab o Jupyter Lab.
�

Juan Pablo · Portafolio de Ciencia de Datos
Documentando el aprendizaje, un dataset a la vez.
�