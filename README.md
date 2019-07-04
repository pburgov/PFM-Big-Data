
<p align="center">
  <img width="460" height="300" src="https://raw.githubusercontent.com/pburgov/PFM-Big-Data/master/images/brexit_small.jpg" style="width: 300px; margin:auto; padding: 0px; border-radius: 8%;">
</p>

# Proyecto Fin del Máster en Big Data y Business Analytics

## Introducción

Para la realización del Proyecto Fin de [Máster Telefónica en Big Data y Business Analytics](https://www.campusbigdata.com/master-en-big-data-aplicado-y-business-analytics),  se ha escogido la opción relativa a los resultados del *Brexit*. Esta elección se justifica en que desde el anuncio por parte de James Cameron en 2013 de la realización del Referendum, la eventual salida del **Reino Unido** de la **UE** ha provocado un gran interés por 2 motivos:
- En primer lugar y fundamentalmente por la posible resaca, que derivada de tal decisión, pudiera sufrir la UE y por tanto España.
- Porque llama poderosamente la atención la tendencia de UK al aislamiento, precisamente en el mundo con tintes globales en el que nos encontramos, y en el que, metafóricamente hablando, un gran número de fronteras se están diluyendo.

#### 1 Objetivo del estudio 

El objetivo principal es el de buscar posibles causas o relaciones comunes, existentes entre los distintos distritos electorales, que hayan decantado el resultado final hacia la salida de la UE.

#### 2 *Datasets* de trabajo

El dataset principal es uno de los 4 propuestos por el claustro del Máster, y que se encuentra disponible en la web [kaggle](https://www.kaggle.com/) bajo el epígrafe [2016 EU Referendum in the United Kingdom ](https://www.kaggle.com/electoralcommission/brexit-results). Dicho *dataset* consta de 2 archivos con formato *csv*:
- **census.csv**: En el se recogen los datos censales de los distintos distritos de Inglaterra, Gales, Escocia e Irlanda del Norte. Los primeros 44 registros del archivo muestran los datos agregados primero por país, luego por región y finalmente por condado. Los 380 registros restantes corresponden a los datos desglosados por distrito. 


<p align="center">
  <img src="https://pburgov.github.io/census.jpg" alt="census">
</p>

- **referendum.csv**: En este fichero se recogen los datos principales de las votaciones realizadas en cada uno de los distritos tales como, asistencia, votos esperados, votos válidos y rechazados,  valores y porcentajes resultantes del escrutinio, etc.


<p align="center">
  <img  src="https://pburgov.github.io/referendum.jpg" alt="referendum">
</p>

Como complementación de este *dataset*, a partir de los datos proporcionados por la web oficial de UK [Nomis - Official Labour Market Statistics](https://www.nomisweb.co.uk) he creado un nuevo archivo también con formato *csv* denominado **social.csv**.
Dicho archivo contiene los siguientes campos:
- <strong>Area_Code</strong>: Código identificativo del distrito. (*String*)
- **jobseeker**: Ratio de gente por distrito en búsqueda de empleo. (*Double*)
- **state_pension**:Ratio de gente que recibe una pensión básica del estado para prevenir la pobreza tras la jubilación. (*Double*)
- **income**: Ratio de gente por distrito que recibe una paga suplementaria para llegar a fin de mes. (*Double*)
- **ESA**: Ratio de gente que recibe una prestación por desempleo, (*Double*)
- **coast**: Indica que el distrito está en la costa. Esta variable parte de la premisa tradicional, quizás errónea, de que los pueblos costeros por su mayor contacto con otras culturas son más abiertos que los pueblos de interior. Éstos por su mayor aislamiento geográfico, se encuentran más encerrados en sí mismos, y por tanto podría contribuir a que el voto de la gente se decantase por el Brexit (*Integer* Valores 1/0)


<p align="center">
  <img  src="https://pburgov.github.io/social.jpg" alt="social">
</p>


#### 3. Ámbito estudio. Inglaterra, Gales y Escocia

El *dataset* **referendum** no recoge los datos segregados por distrito de **Irlanda del Norte**. De la misma manera, el *dataset* **census** no contiene los datos de Gibraltar, por ello se prescinde de ambos, limitándose el estudio a Inglaterra, Gales y Escocia

#### 4. Recursos

El PFM se puede visualizar en el enlace [Proyecto Fin de Máster](https://pburgov.github.io/PFM-BREXIT.html). Asimismo, a través del enlace [PFM-Dashboard](https://public.tableau.com/profile/pedro.burgo#!/vizhome/PFM-BREXIT/Prediccion) es posible acceder al *dashboard* de **Tableau**.