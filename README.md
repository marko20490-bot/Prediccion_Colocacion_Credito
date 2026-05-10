# Análisis del Crédito Bancario en Ecuador (2005–2025)
**Integración de indicadores financieros y macroeconómicos y modelación de series temporales**

## 1. Descripción del proyecto

Este repositorio contiene el desarrollo computacional de un proyecto de investigación académica cuyo objetivo es analizar la evolución del crédito bancario en Ecuador durante el período 2005–2025, integrando información de operaciones crediticias por entidad financiera con indicadores financieros y macroeconómicos.

El proyecto consolida bases de datos históricas de gran volumen, realiza análisis descriptivos y correlacionales, y construye modelos econométricos de series temporales (ARIMA/ARIMAX/SARIMAX) para evaluar la relación entre el crédito y variables exógenas, así como para generar pronósticos de corto y mediano plazo.

## 2. Objetivos

### Objetivo general
Analizar la dinámica del crédito bancario ecuatoriano y su relación con indicadores financieros y macroeconómicos mediante técnicas de análisis de datos y modelación de series temporales.

### Objetivos específicos
- Consolidar una base de datos histórica de operaciones crediticias bancarias entre 2005 y 2025.
- Filtrar y analizar las entidades bancarias privadas de mayor relevancia.
- Integrar indicadores financieros y macroeconómicos al análisis del crédito.
- Evaluar correlaciones y relaciones estadísticas entre variables.
- Estimar modelos ARIMA, ARIMAX y SARIMAX.
- Generar pronósticos anuales del crédito bancario.
- Garantizar reproducibilidad completa de los resultados.

## 3. Datos

### Fuentes
- Archivos anuales `volumen_ene_dic_2005.xlsb` a `volumen_ene_dic_2025.xlsb`.
- Archivo `Indicadores.xlsx` (hojas INDICADORES y BANCOS).

### Variables principales
- `ANIO`, `ENTIDAD`
- `MONTO_OTORGADO`, `NUM_OPERACIONES`
- `ILI`, `ROA`, `ROE`, `MOROSIDAD`
- `DESEMPLEO`, `PIB`, `INFLACION`

## 4. Metodología

1. **Preprocesamiento**: carga, limpieza, estandarización y agregación anual de datos.
2. **Análisis descriptivo**: tendencias del crédito por año y entidad.
3. **Correlación**: análisis no paramétrico (Kendall).
4. **Modelado**: ARIMA/ARIMAX/SARIMAX con variables exógenas.
5. **Validación**: pruebas de estacionariedad, diagnóstico de residuos y métricas de error.
6. **Pronóstico**: proyecciones anuales con intervalos de confianza.

## 5. Resultados

- Base consolidada sin nulos en variables clave.
- Evidencia de relación entre crédito e indicadores macroeconómicos.
- Models ARIMAX/SARIMAX con mejor ajuste que modelos univariados.
- Pronósticos anuales con intervalos de confianza al 95%.

## 6. Reproducibilidad

### Requisitos
- Python >= 3.8

### Librerías
```bash
pip install pandas numpy matplotlib seaborn scipy statsmodels scikit-learn openpyxl pyxlsb
```

### Estructura sugerida
```text
├── data/
├── notebooks/
├── results/
└── README.md
```

### Pasos
1. Clonar el repositorio.
2. Ubicar los datos en la carpeta `data/`.
3. Ejecutar el notebook principal en orden secuencial.
4. Revisar tablas y gráficos generados.

## 7. Autor

Marco Javier Ruiz Torres

## 8. Licencia

Uso académico y de investigación. Se recomienda licencia MIT o CC-BY.
