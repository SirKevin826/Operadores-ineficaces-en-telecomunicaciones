# Operadores-ineficaces-en-telecomunicaciones
Análisis de operadores de telecomunicaciones con el propósito de encontrar a los considerados ineficaces en el mercado de un servicio de telefonía que ha desarrollado una función que brinda a supervisores información sobre los operadores menos eficaces, Además de una evaluación de estrategias comerciales, calidad de servicio y satisfacción del cliente para entender las razones detrás del desempeño deficiente. Se considera que un operador es ineficaz cuando tiene una gran cantidad de llamadas entrantes perdidas ya sean internas y/o externas, así como un tiempo de espera prolongado para las llamadas entrantes. Incluso, hay una señal de ineficacia cuando hay un número reducido de llamadas salientes realizadas por un operador. 

## Archivos

Para la realización de este proyecto, se han utilizado los siguientes archivos que contienen información sobre el uso del servicio de telefonía virtual en la que distribuyen gran cantidad de llamadas entrantes entre varios operadores y/o realizar llamadas salientes a través de sus operadores, asi como la realización de llamadas internas para la comunicación mutua:

El dataset comprimido `telecom_dataset_us.csv` contiene las siguientes columnas:

- `user_id`: ID de la cuenta de cliente
- `date`: fecha en la que se recuperaron las estadísticas
- `direction`: "dirección" de llamada (`out` para saliente, `in` para entrante)
- `internal`: si la llamada fue interna (entre los operadores de un cliente o clienta)
- `operator_id`: identificador del operador
- `is_missed_call`: si fue una llamada perdida
- `calls_count`: número de llamadas
- `call_duration`: duración de la llamada (sin incluir el tiempo de espera)
- `total_call_duration`: duración de la llamada (incluido el tiempo de espera)

El conjunto de datos `telecom_clients_us.csv` tiene las siguientes columnas:

- `user_id`: ID de usuario/a
- `tariff_plan`: tarifa actual de la clientela
- `date_start`: fecha de registro de la clientela


## Metodologías
Para este proyecto, se llevó a cabo lo siguiente:

* Análisis exploratorio de datos
* Descomposición de tareas
* Identificación de operadores ineficaces
* Prueba de hipótesis estadísticas
* Implemenación del plan definido en la descomposición

## Hallazgos y recomendaciones

Durante el desarrollo del proyecto, se han encontrado datos que nos muestran a detalle los problemas de la empresa con sus operadores

* La mayoría de las llamadas son externas y son las que duran más
* En promedio se hacen 1142 s de llamadas externas y 1124 s en promedio son llamadas salientes
* De los 1092 operadores, 503 son eficaces, ya que hay un 50% de tasa de llamadas perdidas, las llamadas salientes en su mayoría tienen una tasa del 0 y 100%, y la duración de la mayoría no duran nada
* De acuerdo con las pruebas Mann-Whitney U y Kolmogorov-Smirnov, SÍ existe una diferencia estadísticamente significativa en las tasas de llamadas perdidas
* Los operadores eficientes logran mantener conversaciones más productivas
* Los operadores ineficientes tienen muchas llamadas muy cortas (posiblemente desconexiones rápidas)

Como resultado se necesitan de acciones inmediatas, para eso se considera lo siguiente:
* Capacitación urgente en manejo de llamadas y técnicas de retención
* Supervisión intensiva con mentores experimentados
* Implementar sistema de alertas cuando la tasa supere el 40%
* Redistribución de carga desde operadores ineficientes a eficientes
* Protocolos mejorados para manejo de llamadas entrantes
* Entrenar en técnicas de conversación efectiva
* Scripts mejorados para llamadas salientes
* Incentivos por mantener conversaciones productivas (>5 minutos)
* Dashboard en tiempo real con métricas clave
* Evaluaciones mensuales de rendimiento
* Plan de carrera diferenciado por nivel de eficiencia



