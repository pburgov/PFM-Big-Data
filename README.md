
 <link rel="stylesheet" type="text/css" media="all" href="https://pburgov.github.io/custom.css" /><title></title>



<p><img src="https://pburgov.github.io/brexit-small.jpg" alt="Brexit" /></p>


![Brexit](./images/brexit-small.jpg)
# Proyecto Fin del Máster en Big Data y Business Analytics
PFM del [Máster Telefónica en Big Data y Business Analytics](https://www.campusbigdata.com/master-en-big-data-aplicado-y-business-analytics) realizado tomando como estudio los resultados del Referendum del *Brexit* en UK.
Se ha utilizado como datasets los proporcionados por la web [kaggle](https://www.kaggle.com/) bajo el epígrafe [ 2016 EU Referendum in the United Kingdom](https://www.kaggle.com/electoralcommission/brexit-results)

## <a id='1.2'> </a>1 Introducción<span><a  href='#titulo'> &#8593; Menú</a></span>

Para la realización del Proyecto Fin de Máster, he escogido la opción relativa a los resultados del Brexit. Esta elección se justifica en que desde el anuncio por parte de James Cameron en 2013 de la realización del Referendum, la eventual salida del **Reino Unido** de la **UE** me ha provocado un gran interés por 2 motivos:
- En primer lugar y fundamentalmente por la posible resaca, que derivada de tal decisión, pudiera sufrir la UE y por tanto España.
- Porque llama poderosamente la atención la tendencia de UK al aislamiento, precisamente en el mundo con tintes globales en el que nos encontramos, y en el que, metafóricamente hablando, un gran número de fronteras se están diluyendo.


#### <a id="1.1"> </a>1.1 Objetivo del estudio <span><a  href="#titulo"> &#8593; Menú</a></span>

El objetivo principal es el de buscar posibles causas o relaciones comunes, existentes entre los distintos distritos electorales, que hayan decantado el resultado final hacia la salida de la UE.

### <a id="1.2"> </a>1.2 <em>Datasets</em> de trabajo<span><a  href="#titulo"> &#8593; Menú</a></span>

#### <a id="1.2.1"> </a>1.2.1 Descripción<span><a  href="#titulo"> &#8593; Menú</a></span>

El dataset principal es uno de los 4 propuestos por el claustro del Máster, y que se encuentra disponible en la web [kaggle](https://www.kaggle.com/) bajo el epígrafe [2016 EU Referendum in the United Kingdom ](https://www.kaggle.com/electoralcommission/brexit-results). Dicho *dataset* consta de 2 archivos con formato *csv*:
- **census.csv**: En el se recogen los datos censales de los distintos distritos de Inglaterra, Gales, Escocia e Irlanda del Norte. Los primeros 44 registros del archivo muestran los datos agregados primero por país, luego por región y finalmente por condado. Los 380 registros restantes corresponden a los datos desglosados por distrito. 

![census](https://pburgov.github.io/census.jpg)

- **referendum.csv**: En este fichero se recogen los datos principales de las votaciones realizadas en cada uno de los distritos tales como, asistencia, votos esperados, votos válidos y rechazados,  valores y porcentajes resultantes del escrutinio, etc.

![referendum](![census](https://pburgov.github.io/referendum.jpg))

Como complementación de este *dataset*, a partir de los datos proporcionados por la web oficial de UK [Nomis - Official Labour Market Statistics](https://www.nomisweb.co.uk) he creado un nuevo archivo también con formato *csv* denominado **social.csv**.
Dicho archivo contiene los siguientes campos:
- <strong>Area_Code</strong>: Código identificativo del distrito. (*String*)
- **jobseeker**: Ratio de gente por distrito en búsqueda de empleo. (*Double*)
- **state_pension**:Ratio de gente que recibe una pensión básica del estado para prevenir la pobreza tras la jubilación. (*Double*)
- **income**: Ratio de gente por distrito que recibe una paga suplementaria para llegar a fin de mes. (*Double*)
- **ESA**: Ratio de gente que recibe una prestación por desempleo, (*Double*)
- **coast**: Indica que el distrito está en la costa. Esta variable parte de la premisa tradicional, quizás errónea, de que los pueblos costeros por su mayor contacto con otras culturas son más abiertos que los pueblos de interior. Éstos por su mayor aislamiento geográfico, se encuentran más encerrados en sí mismos, y por tanto podría contribuir a que el voto de la gente se decantase por el Brexit (*Integer* Valores 1/0)

![social](![census](https://pburgov.github.io/social.jpg))

