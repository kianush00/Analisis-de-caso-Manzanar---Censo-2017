# Análisis de caso Manzanar - Censo 2017 - Hito 3
<img src="https://upload.wikimedia.org/wikipedia/commons/4/46/Censo_2017.png" width=300>

## Descripción
El presente proyecto espera resolver la incertidumbre que se genera por la falta de datos del CENSO por medio de herramientas de minería de datos. De esta manera, se ahorra trabajo a los futuros analistas de datos que deseen utilizar esta nueva información. Para ello se plantea la posibilidad de obtener la clase de la manzana, dígase el tipo de entidad (campo, pueblo, caserío, etc.) que esta representa para poder completar los datos para futuros análisis. Además se busca predecir el tipo de área rural o urbana de una manzana.


## Estructura del repositorio
```bash
.
├── data                                # Datos utilizados
│   ├── Censo_Filtrado_Hito_1.csv       # Datos crudos iniciales del Censo 2017
│   ├── resultado_hito1.csv             # Datos procesados del Censo 2017
├── resources                           # Recursos utilizados en el proyecto
│   ├── hito3_G4_presentacion.pdf       # Presentación del proyecto
│   ├── hito3_G4_informe.pdf            # Informe IEEE del proyecto
├── src                                 # Código fuente almacenado
│   ├── hito3_G4_proyecto.ipynb         # Código fuente del proyecto
│   ├── hito3_G4_proyecto.html          # Exportación del código fuente
├── README.md                           # Descripción del proyecto
```

## Herramientas

Para poder ejecutar los comandos del código fuente en un entorno local, es necesario instalar las siguientes herramientas:

### Anaconda
Anaconda facilita la instalación de bibliotecas necesarias para la ejecución del código fuente. Una vez instalada esta herramienta en su entorno local, se deben seguir estos pasos:

 1. Abrir aplicación Anaconda prompt
 2. Ejecutar comando: ```conda install [biblioteca]```

Bibliotecas utilizadas en el código fuente: *numpy, scikit-learn, pandas, matplotlib, seaborn*

### Jupyter
Jupyter notebook (viene con anaconda) es una aplicación web que se utilizará para ejecutar el código fuente del proyecto.

Para cargar y editar el archivo *.ipynb* que contiene el código fuente, se debe abrir la terminal y ejecutar ```jupyter notebook```. Esto abrirá el navegador donde se puede buscar el archivo .ipynb dentro del directorio. 

Para ejecutar un bloque de código del notebook se puede utilizar el atajo *Shift-Enter*.


## Hoja de ruta
1. En avances anteriores se intentó predecir algún tipo de indicador de pobreza, pero no fue posible ya que la pobreza no posee una correlación directa con la calidad de la vivienda, por lo que se requerirían otras variables como la situación económica de la población. Debido a que se tuvo que descartar esa idea, también se descartaron los gráficos de torta de inmigración y pueblos indígenas del país.

2. En los primeros avances se visualizaron datos que no poseían una relación directa con los problemas, como el "summary" de todos los atributos, por lo que fueron descartados.

3. Para resolver los problemas propuestos se tuvieron que desechar muchos atributos que se referían al tipo de materialidad de las viviendas de una manzana, ya que en el dataset original estos atributos derivan de forma directa en la calidad de materialidad, por lo que resultan ser redundantes para la implementación.

4. Antes de haber empezado a avanzar con el proyecto, se pudo haber elegido un dataset que entregue datos de personas individuales en vez de las manzanas, ya que entregan información con mayor variedad, como su situación económica, grado de escolaridad, entre otros factores. El problema que posee el dataset de personas individuales es su gran tamaño, teniendo en cuenta que cada fila corresponde a un habitante, por lo que en ese caso se podría restringir a una región en específico.

5. Se pudo haber agregado atributos provenientes de otros datasets para poder resolver el primer problema con una mayor precisión, pero hasta el momento no se halló más información al respecto.

## Autores
- Alonso Rojas [@AlonsoRojas98](https://gitlab.com/AlonsoRojas_98)
- Diego Vera [@DiegoVeraSuazo](https://github.com/DiegoVeraSuazo)
- Arturo Avendaño [@ArturoAvendano](https://github.com/ArturoAvendano)
- Kianush Atighi-Moghaddam [@kianush00](https://github.com/kianush00)

## Estado del proyecto
El proyecto actualmente se encuentra a disposición de aceptar cambios y propuestas de mejora con tal de sacarle mayor provecho al análisis de la población por medio de la minería de datos.
