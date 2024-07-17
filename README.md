# Proyecto 2: Análisis de datos de las telecomunicaciones Argentina:

## Contexto de este proyecto
En los últimos años, la conectividad a internet se ha convertido en un pilar fundamental para el desarrollo económico y social de Argentina. La expansión de la red y la mejora de los servicios de internet han sido posibles gracias a la colaboración entre el sector público y privado. Esta sinergia ha permitido obtener resultados significativos, como la expansión de la red a todas las regiones del país, la mejora de las condiciones del servicio, y el aumento de la velocidad promedio de conexión.

Expansión y Mejora del Servicio de Internet

El Instituto Nacional de Estadística y Censos (INDEC) reporta un aumento significativo en el uso de internet, que pasó del 82% al 90% de la población en los últimos años. Este incremento refleja no solo la mayor disponibilidad de servicios de internet, sino también la creciente necesidad de conectividad en todos los aspectos de la vida cotidiana, especialmente en un contexto de pandemia.

La Iniciativa REFEFO

Un ejemplo destacado de la política de expansión es el Proyecto REFEFO (Red Federal de Fibra Óptica). Esta iniciativa ha sido crucial para llevar internet de alta velocidad a regiones que anteriormente no contaban con este servicio. REFEFO ha permitido que comunidades rurales y áreas menos desarrolladas tengan acceso a una conectividad robusta, facilitando así el desarrollo económico y mejorando la calidad de vida de sus habitantes.

Impacto de la Pandemia en la Conectividad
La pandemia de COVID-19 ha resaltado la importancia de una infraestructura de internet confiable y de alta calidad. Con el incremento del teletrabajo, la educación a distancia y el entretenimiento digital, la demanda de servicios de internet ha crecido exponencialmente. Este contexto ha acelerado la implementación de mejoras en la red y ha incentivado nuevas inversiones en infraestructura digital.



Los datos económicos son esenciales para evaluar el impacto financiero del crecimiento de la conectividad en Argentina. Al analizar la correlación entre el aumento del uso de internet y los ingresos generados, se pueden identificar tendencias y oportunidades para futuras inversiones.

## Conceptos relevantes para el análisis de los datos

ADSL: ADSL (Asymmetric Digital Subscriber Line) es una tecnología de conexión a Internet de banda ancha que utiliza líneas telefónicas para transmitir datos. Proporciona una velocidad de descarga más rápida en comparación con la velocidad de carga. Es ampliamente utilizado en hogares y pequeñas empresas.

Cablemodem: El cablemodem es un dispositivo que permite la conexión a Internet a través de las redes de cable de televisión. Utiliza la infraestructura de televisión por cable para transmitir datos de alta velocidad. Es una opción popular para conexiones de Internet de alta velocidad en hogares y negocios.

Fibra óptica: La fibra óptica es una tecnología de transmisión de datos que utiliza hilos delgados de vidrio o plástico para transmitir señales de luz. Proporciona velocidades de conexión extremadamente rápidas y mayor capacidad de ancho de banda en comparación con otras tecnologías. La fibra óptica es conocida por su alta velocidad y estabilidad, y es utilizada en conexiones de Internet de alta velocidad y redes de telecomunicaciones.

Wireless: Wireless, también conocido como conexión inalámbrica, se refiere a la tecnología que permite la transmisión de datos sin cables físicos. Utiliza ondas de radio o señales de infrarrojos para enviar y recibir datos. Las conexiones inalámbricas son ampliamente utilizadas en dispositivos móviles, como teléfonos inteligentes, tabletas y computadoras portátiles, así como en redes Wi-Fi para acceder a Internet.

Mbps (Media de bajada): Mbps (Megabits por segundo) es una unidad de medida utilizada para expresar la velocidad de transferencia de datos en una conexión a Internet. Representa la cantidad de megabits que pueden ser transferidos por segundo. La velocidad de bajada se refiere a la velocidad a la cual los datos pueden ser descargados desde Internet hacia el dispositivo del usuario. Cuanto mayor sea el valor de Mbps, más rápido será el proceso de descarga de datos.

Datos Económicos y Análisis de Ingresos:
Para entender mejor los ingresos generados por los accesos a internet, se ha incorporado un conjunto de datos económicos extraídos de la página www.Investing.com. Este dataset incluye registros de los últimos 10 años del valor del dolar blue, agrupados por trimestre y promediando los valores de los tres meses. Aunque los números son estimaciones, proporcionan una visión general de la evolución económica asociada con el acceso a internet.

## ETL

Para realizar este proyecto se realizó un etl donde los datos fuerom extraidos de la página ofical del enacom https://indicadores.enacom.gob.ar/datos-abiertos y limpiados con python  y pandas.

consideraciones:

-En el caso de los valores faltantes para variables no categoricas se decicidió relllenar con '0' como valor, entendiendo que si faltaban valores es proque no existen.

-Al ser una fuente de datos oficial Los valores considerados outliers seran mencionados, pero no serán ni eliminados bajo ningún punto de vista.


## EDA

El analisis exploratorio de los datos fue realizado en un notebook de jupyter, en el se profundizó todas las cuestiones relativas a los datasets implementados.

los datasets que utilizaremos serán:

- df_definitivol: Conjunto de datos que tiene cantidad de accesos por tecnologia y velocidad por provincia, penetracion cada 100 hogares,penetracion cada 100 habitantes'
- df_ingresos_dolar: tiene los ingresos por trimestre en pesos,adicionalmente agregó el valor de dolar blue(dolar libre en argentina, no es el dolar oficial pero es el valor de referencia que rige en los mercados) para poder tener una idea de como fueron los ingresos en dolares
- df_localidades_tecnologia: es un recuento de las tegnologias en cada localidad
- Totales_VMD: es un promedio de la velocidad media de bajada por trimestre

## Tecnologías utilizadas en el proyecto
-Pyhon (librerias: Pandas, seaborn y matplotlib)
-Powerbi 

## Conclusión
La mejora y expansión de los servicios de internet en Argentina han sido posibles gracias a una colaboración efectiva entre el sector público y privado. Iniciativas como REFEFO han jugado un papel crucial en esta transformación, y la pandemia ha acelerado la necesidad de una conectividad robusta. Analizar estos desarrollos desde una perspectiva económica proporciona una base sólida para futuras inversiones y políticas públicas que continúen mejorando la infraestructura digital del país.