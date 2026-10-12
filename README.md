# StreamView Analytics — Visualización de Datos

**Proyecto académico | Ingeniería Informática — Mención Ciencia de Datos**

Repositorio correspondiente al desarrollo del proyecto **StreamView Analytics**, realizado para la asignatura de Visualización de Datos.

## 1. Descripción del proyecto

StreamView Analytics es un proyecto de análisis y visualización de datos orientado a transformar información de un catálogo audiovisual en indicadores, gráficos interactivos y herramientas de apoyo a la toma de decisiones.

La solución utiliza **Python en Google Colab** para realizar el análisis exploratorio, limpieza y preparación de datos, y **Microsoft Power BI** para construir dashboards interactivos dirigidos a diferentes áreas de una organización.

El objetivo principal es facilitar la interpretación de datos mediante técnicas de Visual Analytics, indicadores clave de desempeño (KPIs) y principios de Data Storytelling.

## 2. Objetivos

### Objetivo general

Diseñar e implementar una solución de visualización de datos que permita analizar el catálogo audiovisual, identificar patrones relevantes y apoyar la toma de decisiones estratégicas y operativas.

### Objetivos específicos

- Realizar un análisis exploratorio de los conjuntos de datos.
- Identificar valores faltantes, duplicados, distribuciones y valores atípicos.
- Integrar y preparar los datos para su posterior análisis.
- Definir KPIs asociados a necesidades de distintas áreas de negocio.
- Construir dashboards interactivos mediante Power BI.
- Aplicar principios de diseño visual y Data Storytelling.
- Identificar oportunidades de mejora y limitaciones de la información disponible.

## 3. Tecnologías utilizadas

| Tecnología | Propósito |
|---|---|
| Python | Procesamiento y análisis de datos |
| Google Colab | Desarrollo y ejecución del notebook |
| Pandas | Manipulación y limpieza de datos |
| NumPy | Operaciones numéricas |
| Matplotlib | Visualización exploratoria |
| Seaborn | Análisis gráfico de distribuciones |
| Microsoft Power BI | Construcción de dashboards interactivos |
| DAX | Definición de medidas e indicadores |
| Power Query | Transformación y preparación de datos |
| GitHub | Versionamiento y documentación |

## 4. Fuentes de datos

El proyecto utiliza dos conjuntos de datos audiovisuales:

- **Netflix Movies Detailed up to 2025**
- **Netflix TV Shows Detailed up to 2025**

Estos contienen información sobre películas y series, incluyendo variables como:

- Título y tipo de contenido.
- País e idioma.
- Fecha y año.
- Popularidad.
- Valoración promedio.
- Cantidad de votos.
- Presupuesto y recaudación, cuando corresponde.

Después de la preparación y consolidación, el conjunto de datos contiene **31.991 registros**, distribuidos en:

| Tipo de contenido | Registros |
|---|---:|
| Películas | 16.000 |
| Series | 15.991 |
| **Total** | **31.991** |

Durante el proceso de limpieza se identificaron y eliminaron 9 registros duplicados de series mediante el identificador `show_id`.

## 5. Metodología de trabajo

### Etapa 1: Análisis exploratorio de datos (EDA)

Se utilizó Google Colab para analizar la estructura y calidad de los conjuntos de datos.

Las actividades principales fueron:

- Inspección de columnas y tipos de datos.
- Análisis de estadísticas descriptivas.
- Identificación de valores nulos.
- Detección de registros duplicados.
- Exploración de distribuciones.
- Identificación de valores atípicos.
- Comparación de variables relevantes.

Este proceso permitió identificar características y limitaciones que posteriormente influyeron en la construcción de los dashboards.

### Etapa 2: Limpieza y preparación

Se realizaron transformaciones para mejorar la consistencia de los datos:

- Eliminación de duplicados.
- Normalización de formatos.
- Revisión de variables numéricas y categóricas.
- Tratamiento de valores faltantes según su contexto.
- Integración de películas y series en un catálogo consolidado.
- Exportación de datos preparados para Power BI.

Los campos financieros se utilizan considerando su disponibilidad y validez. No se reemplazan automáticamente los presupuestos o ingresos faltantes mediante promedios.

### Etapa 3: Construcción de dashboards

Se desarrollaron cinco dashboards especializados en Power BI, organizados según las necesidades de distintas áreas.

**1. Directorio y Gerencia General**

Proporciona una visión ejecutiva del catálogo audiovisual mediante indicadores de valoración, popularidad y desempeño financiero.

KPI principal: ROI global, definido como la relación entre recaudación y presupuesto.

**2. Gerencia de Marketing**

Permite analizar la popularidad y valoración de los contenidos para identificar oportunidades promocionales.

KPI principal: popularidad promedio.

Incluye un ranking Top 10 de oportunidades promocionales, orientado a identificar títulos con buena valoración y popularidad relativamente baja.

**3. Gerencia de Contenidos y Adquisición**

Facilita el análisis de variables financieras y la identificación de títulos que requieren revisión.

KPI principal: proporción de presupuesto asociada a películas de bajo desempeño.

Incluye un Top 10 de inversiones prioritarias para revisión, basado en las brechas entre presupuesto y recaudación.

**4. Gerencia de Producto**

Analiza la composición del catálogo audiovisual y su diversidad idiomática.

KPI principal: porcentaje de contenido en idiomas distintos del inglés.

Permite examinar la distribución del catálogo para apoyar decisiones de visibilidad y navegación.

**5. Data & Analytics**

Supervisa la calidad y disponibilidad de la información utilizada en el proyecto.

KPI principal: completitud del catálogo consolidado.

Incluye análisis de valores faltantes, cobertura de campos críticos y excepciones.

## 6. KPIs principales

Los dashboards incorporan indicadores acompañados de metas de referencia y estados de cumplimiento.

| Área | KPI | Valor global | Meta o límite |
|---|---|---|---|
| Directorio | ROI global | 2,92x | 2,50x |
| Marketing | Popularidad promedio | 42,63 | 50 |
| Contenidos y Adquisición | Exposición presupuestaria a bajo desempeño | 6,4% | Máximo 10% |
| Producto | Contenido no inglés | 57% | 40% |
| Data & Analytics | Completitud global | 72% | 90% |

**Importante:** las metas fueron propuestas con fines académicos y de seguimiento. No representan objetivos institucionales oficiales.

Los resultados corresponden al contexto global de análisis y pueden variar según los filtros aplicados.

## 7. Diseño visual y Data Storytelling

El proyecto aplica principios de visualización de datos para facilitar la comprensión de información compleja.

Se utiliza la siguiente secuencia narrativa:

**Contexto → KPI → Evidencia → Priorización → Acción**

Esta estructura permite identificar una situación, comprender sus causas y reconocer posibles decisiones.

Entre los principios aplicados se encuentran:

- Jerarquía visual de indicadores.
- Uso de gráficos según el propósito analítico.
- Consistencia de colores y etiquetas.
- Reducción de elementos visuales innecesarios.
- Interactividad mediante filtros y segmentadores.
- Organización de información según la audiencia.

## 8. Estructura del repositorio

La siguiente es la estructura recomendada para organizar los archivos del proyecto:

```text
VisualizacionDeDatos_Encargo2/
│
├── data/
│   ├── Netflix_Movies.csv
│   ├── Netflix_TV_Shows.csv
│   └── StreamView_Catalogo_Master_Limpio.xlsx
│
├── notebooks/
│   └── VisualizacionDeDatos_Encargo1.ipynb
│
├── dashboard/
│   └── VisualizacionDeDatos_BI_encargo2_revisar.pbix
│
├── images/
│   └── Infografia_StreamView.png
│
├── docs/
│   ├── Informe_Tecnico_StreamView_EP3.pdf
│   └── Presentacion_StreamView.pptx
│
└── README.md
```

**Nota:** esta estructura es una propuesta de organización. Los nombres y las rutas deben ajustarse a los archivos efectivamente incorporados al repositorio.

## 9. Requisitos de ejecución

Para reproducir el análisis se recomienda contar con:

- Python 3.
- Google Colab o Jupyter Notebook.
- Bibliotecas Pandas, NumPy, Matplotlib, Seaborn y XlsxWriter.
- Microsoft Power BI Desktop.
- Acceso a los conjuntos de datos originales.

Instalación de las bibliotecas principales:

```bash
pip install pandas numpy matplotlib seaborn xlsxwriter
```

## 10. Pasos para reproducir el proyecto

**Paso 1.** Obtener los datasets originales de películas y series.

**Paso 2.** Abrir el notebook de análisis exploratorio en Google Colab o Jupyter Notebook.

**Paso 3.** Verificar las rutas de acceso a los archivos de origen y ejecutar las celdas de preparación y análisis.

**Paso 4.** Comprobar los resultados de limpieza, incluyendo la eliminación de duplicados y la consolidación de los 31.991 registros.

**Paso 5.** Exportar el catálogo consolidado a Excel.

**Paso 6.** Abrir el archivo `.pbix` en Power BI Desktop.

**Paso 7.** Verificar la conexión al archivo consolidado y actualizar el modelo cuando corresponda.

**Paso 8.** Revisar los KPIs, filtros, segmentadores y visualizaciones de cada dashboard.

La ejecución puede requerir actualizar las rutas de origen de los datos según el entorno utilizado.

## 11. Limitaciones del proyecto

Los resultados deben interpretarse considerando las características de los datos disponibles.

- La variable `popularity` es un índice relativo y no representa reproducciones reales de usuarios.
- Los valores de `budget` corresponden a presupuestos de producción y no a costos de adquisición o licenciamiento.
- La variable `revenue` representa recaudación y no utilidad neta.
- El ROI utilizado sigue la definición establecida para el caso académico.
- Las brechas entre presupuesto y recaudación no representan necesariamente pérdidas contables.
- No se dispone de información suficiente para calcular indicadores reales de retención, abandono o engagement de usuarios.
- Algunos campos presentan valores faltantes o cobertura desigual.

Por estas razones, las recomendaciones se presentan dentro del alcance de los datos disponibles.

## 12. Conclusiones

El desarrollo de StreamView Analytics permitió integrar técnicas de análisis exploratorio, preparación de datos y visualización interactiva en una solución orientada a distintas necesidades organizacionales.

La implementación de KPIs y dashboards especializados facilita la identificación de tendencias, oportunidades promocionales, posibles riesgos financieros y problemas de calidad de datos.

Asimismo, la aplicación de principios de Data Storytelling contribuye a transformar los resultados analíticos en información comprensible y orientada a decisiones.

El proyecto demuestra la importancia de combinar calidad de datos, análisis técnico y comunicación visual para generar información útil a partir de fuentes audiovisuales.

## 13. Contexto académico

**Proyecto:** StreamView Analytics

**Asignatura:** Visualización de Datos

**Programa:** Ingeniería Informática — Mención Ciencia de Datos

**Evaluación:** EP3 — Visualización y análisis de datos

**Integrantes:**
- Diego Améstica
- Agustín Cáceres

**Docente:** Felipe Eduardo Cabrera Orella

---

*Repositorio desarrollado con fines académicos y educativos.*
