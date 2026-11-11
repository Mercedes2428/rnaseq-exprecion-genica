# Proyecto de Análisis de Expresión Génica de Datos de Secuenciación de ARN
El propósito de este proyecto es examinar un conjunto de muestras biológicas con el objetivo de analizar su expresión génica empleando el método denominado RNA-Seq (Secuenciación de ARN), mediante distintas técnicas y herramientas bioinformáticas adecuadas haciendo uso de métodos estadístico que nos permitirán detectar aquellos genes que están diferencialmente expresados en distintas condiciones experimentales. De igual forma, se examinarán gráficos y tablas de resultados para el análisis de expresión génica con el objetivo de detectar patrones de secuenciación y su relación con las condiciones biológicas de las muestras. 

**Objetivo general:** 

- Analizar datos de RNA-Seq para identificar diferencias de expresión génica entre dos condiciones experimentales mediante un flujo de trabajo reproducible.

**Objetivos específicos:**

- Procesar los datos de secuenciación de ARN (RNA-Seq) mediante herramientas bioinformáticas.
- Identificar los genes diferencialmente expresados entre las diferentes condiciones experimentales mediante análisis estadísticos.
- Interpretar los patrones de expresión génica mediante gráficos y tablas de resultados.

**Contextualización**

El análisis de expresión génica por secuenciación de ARN, conocido como RNA‑Seq, se ha vuelto una herramienta esencial en la investigación molecular. RNA‑Seq permite identificar cambios en la actividad de genes cuando las condiciones biológicas cambian. Kreis y compañía en 2024 estudiaron la infección por Clostridioides difficile en ratones. Usaron RNA‑Seq para observar la expresión génica del patógeno y del ratón al mismo tiempo. Los investigadores hallaron 61 ARN no codificantes que cambiaron en la bacteria durante la infección. También vieron alteraciones en genes del ratón relacionados con la respuesta inflamatoria. Estos hallazgos muestran la utilidad de RNA‑Seq para entender los mecanismos moleculares en distintas condiciones biológicas.

En estudios recientes, Liu y compañía en 2025 estudiaron la expresión génica de pacientes con diabetes tipo 2. Usaron RNA‑Seq del transcriptoma completo. Compararon sangre de cinco pacientes con diabetes y cinco personas sanas. Encontraron 411 ARN mensajeros, 500 ARN largos no codificantes, 356 ARN circulares y 67 microARN con expresión diferente. Los análisis funcionales revelaron rutas moleculares vinculadas a la respuesta inmunitaria, la inflamación y el metabolismo. Estos resultados resaltan la importancia del procesamiento bioinformático y del análisis estadístico de los datos de RNA‑Seq para detectar patrones de expresión génica y entender su relación con procesos fisiológicos y patológicos.

Degen y Medo en 2025 evaluaron la reproducibilidad de análisis de expresión génica con RNA‑Seq. Usaron 18 000 experimentos de submuestreo de 18 conjuntos de datos reales. Descubrieron que estudios con pocas réplicas biológicas pueden tener problemas para reproducir resultados. Esto subraya la necesidad de organizar bien los datos y usar procedimientos estadísticos rigurosos. En este contexto, el proyecto propuesto busca crear y documentar en GitHub un análisis de expresión génica con R y DESeq2. El objetivo es procesar datos de RNA‑Seq, identificar genes diferencialmente expresados entre condiciones experimentales e interpretar sus patrones con tablas y gráficos. Así se promueve el uso de herramientas bioinformáticas y la reproducibilidad de los análisis transcriptómicos.

**Instrucciones**

1. Ingresar al repositorio de GitHub y descargar los archivos del proyecto, que incluyen los datos de ejemplo, los códigos de análisis y la documentación.

2. Instalar R, Python y las bibliotecas necesarias, especialmente DESeq2, para el procesamiento y análisis estadístico de los datos.

3. Organizar los datos de RNA-Seq en una matriz de conteos génicos y un archivo de metadatos que identifique las muestras y sus condiciones experimentales.

4. Utilizar los scripts disponibles en el repositorio para normalizar los datos e identificar los genes diferencialmente expresados entre las condiciones experimentales.

5. Examinar los gráficos de volcán, mapas de calor y análisis de componentes principales (PCA) para observar los patrones de expresión génica.

6. Analizar las tablas y representaciones gráficas para reconocer diferencias en la expresión de los genes y su posible relación con las condiciones biológicas estudiadas.

7. Registrar los procedimientos, resultados y conclusiones en el repositorio de GitHub, facilitando la reproducibilidad y el acceso a la información.

**Métodología de análisis**

El proyecto se hará con un enfoque de bioinformática y estadística para analizar la expresión de genes a partir de datos de secuenciación de ARN. Se usará GitHub para organizar, documentar y compartir el proyecto. R y DESeq2 se usarán para procesar y analizar estadísticamente los datos.

**1. Creación y organización del repositorio en GitHub**

Se creará un repositorio en GitHub llamado rnaseq-expresión-génica. Este repositorio tendrá los datos, los códigos, los resultados y la documentación del proyecto. Se añadirá un archivo README.md con la descripción del estudio, los objetivos y las instrucciones de uso.

**2. Preparación del conjunto de datos**

Se usarán datos simulados de RNA-Seq que incluyen 500 genes y 12 muestras. Se dividirán en seis muestras de control y seis muestras de tratamiento. Los datos se organizarán en una matriz de conteos y en un archivo de metadatos que indique las condiciones experimentales.

**3. Procesamiento y normalización de los datos**

Se usará R y el paquete DESeq2 de Bioconductor para procesar y normalizar los datos. Este proceso controlará diferencias por profundidad de secuenciación y facilitará comparar las muestras.

**4. Análisis de expresión génica diferencial**

Se hará un análisis con DESeq2 para encontrar genes con diferencias significativas de expresión entre control y tratamiento. Se usarán criterios de padj menor a 0.05 y de cambio absoluto log2FC mayor a 1.

**5. Visualización e interpretación de resultados**

Los resultados se mostrarán con gráficos de volcán, mapas de calor y PCA. Estas herramientas ayudarán a ver los genes sobreexpresados y subexpresados, a identificar patrones y a explorar similitudes y diferencias entre las muestras.

**6. Documentación y publicación de resultados en GitHub**

Se incluirán en el repositorio los resultados del análisis, las tablas estadísticas, los gráficos y los códigos usados. También se actualizará el archivo README.md con la metodología, las instrucciones de ejecución y las conclusiones. Esto permitirá que otros usuarios reproduzcan el estudio y accedan a la información.

**7. Evaluación de las limitaciones**

Se revisarán limitaciones relacionadas con la calidad de los datos, la variabilidad experimental y los métodos estadísticos usados. Como las muestras son simuladas, los resultados se usarán con fines educativos y metodológicos, sin sacar conclusiones biológicas sobre organismos o enfermedades reales.

**Estructura de la carpeta en GitHub**

rnaseq-expresion-genica/
│
├── README.md
├── LICENSE
├── .gitignore
│
├── data/
│   └── ejemplo/
│       ├── conteos.tsv
│       └── metadatos.tsv
│
├── scripts/
│   ├── instalar_dependencias.R
│   ├── analisis_rnaseq.R
│   └── validar_entradas.py
│
├── resultados/
│
├── docs/
│   ├── metodologia.md
│   ├── datos_reales.md
│   └── interpretacion.md
│
├── tests/
│   └── test_validar_entradas.py
│
└── .github/
    └── workflows/
        └── validacion.yml

**Descripción de las carpetas y archivos en GitHub** 

- README.md	Presentación, propósito, objetivos, metodología e instrucciones del proyecto.
- data/	Matriz de conteos génicos y metadatos de las muestras biológicas.
- scripts/	Códigos de R y Python para el análisis y la validación de datos.
- resultados/	Tablas estadísticas, genes diferencialmente expresados y gráficos generados.
- docs/	Documentación científica, metodología e interpretación de resultados.
- tests/	Pruebas para verificar el funcionamiento del código.
- github/workflows/	Configuración de pruebas automatizadas en GitHub.
- LICENSE	Condiciones de uso y distribución del proyecto.
- .gitignore Archivos que Git no debe incorporar al repositorio.

**Enlaces de descargas y herramientas necesarias** 

- **GitHub:** https://github.com/
- **R:** https://cran.r-project.org/
- **RStudio:** https://posit.co/downloads/
- **Bioconductor:** https://bioconductor.org/install/
- **DESeq2:** https://bioconductor.org/packages/DESeq2/
- **Python:** https://www.python.org/downloads/
- **Visual Studio Code:** https://code.visualstudio.com/download
- **Git:** https://git-scm.com/downloads
- **ggplot2:** https://ggplot2.tidyverse.org
- **pheatmap:** https://cran.r-project.org/web/packages/pheatmap/index.html
- **nf-core/rnaseq:** https://nf-co.re/rnaseq

**Referencias Bibliográficas** 

Degen, P. M., & Medo, M. (2025). Replicability of bulk RNA-Seq differential expression and enrichment analysis results for small cohort sizes. PLOS Computational Biology, 21(5), e1011630. https://doi.org/10.1371/journal.pcbi.1011630

Kreis, V., Toffano-Nioche, C., Denève-Larrazet, C., Marvaud, J.-C., Garneau, J. R., Dumont, F., van Dijk, E. L., Jaszczyszyn, Y., Boutserin, A., D'Angelo, F., Gautheret, D., Kansau, I., Janoir, C., & Soutourina, O. (2024). Dual RNA-seq study of the dynamics of coding and non-coding RNA expression during Clostridioides difficile infection in a mouse model. mSystems, 9(12), e00863-24. https://doi.org/10.1128/msystems.00863-24

Liu, F., Peng, A., Zhu, X., & Wang, G. (2025). Differential expression and correlation analysis of whole transcriptome for type 2 diabetes mellitus. Frontiers in Endocrinology, 16, Article 1541261. https://doi.org/10.3389/fendo.2025.1541261

