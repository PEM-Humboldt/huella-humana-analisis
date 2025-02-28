Cálculo Huella espacial humana
================
En esta sección se guardan los códigos relacionados con  la construcción de la huella espacial humana: 

1. 00_InsumosGenerales.R: En este código se preparan los insumos base para correr el IHEH. Dichos insumos no cambian comunmente, ya que son los que definen los parametros generales de la misma; proyección, extensión.
Además se preparan:
    - Capas constantes con los parametros generales como: Ecosistemas potenciales y Tiempo de Intervención.
    - Tabla de consulta para la definición de las clases de biomasa y uso de tierra
2. 01_Insumosxhuella.R:Se preparan los insumos necesarios para correr el IHEH y se almacenan en la carpeta de resultados intermedios, Res_Intermedios
3. 02_HuellaHumana_Diaz.R:En este código calcula la huella 2018 replicando los pasos de los modelos de ArcMap de Julian Díaz. Por motivos computacionales fue necesario hacer hacer algunas modificaciones.
4. 03_HuellaHumana_adaptada.R:En este código calcula la huella con el método de ecosistemas. Esta incluye los siguiientes cambios.
    - Variables continuas como continuas
    - Remoción de variables no escenciales para el cálculo.
5. 04_Comparar entre versiones: Código incompleto para comparar entre versiones


## versiones de los paquetes usados

En el momento de la elaboración de los códigos las version de R y de los paquetes necesarios para los códigos fue. 

R version 4.4.1 (2024-06-14 ucrt)
- dplyr_1.1.4  
- terra_1.7-83 
- sf_1.0-19
- raster_3.6-30   
- sp_2.1-4        
- lubridate_1.9.3 
- forcats_1.0.0   
- stringr_1.5.1   
- purrr_1.0.2
- readr_2.1.5     
- tidyr_1.3.1     
- tibble_3.2.1    
- ggplot2_3.5.1   
- tidyverse_2.0.0


## Organizar directorio de trabajo

Los datos para correr los códigos están almacenados
[aquí](https://drive.google.com/file/d/1YQjFb3u8uJ7UmWHlNncM_UXtJ_gJcOmz/view?usp=drive_link)
Una vez descargada y descomprimida la carpeta, reemplaze la carpeta “Datos” en el directorio Datos del proyecto.
El directorio del proyecto está organizado de esta manera que facilita la ejecución del
código:

    Codigos
    │-  00_InsumosGenerales.R
    │-  01_Insumosxhuella.R
    │-  02_HuellaHumana_Diaz.R
    │-  03_HuellaHumana_adaptada.R
    │-  04_Comparar entre versiones.R
    │    
    └-Datos
    │ │
    │ └- replaze aquí los datos que  descargué 
    │ 
    |
    └- Res_Intermedios
    |
    └- Resultados

