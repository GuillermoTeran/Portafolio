# Portafolio
Resúmen de proyectos realizados en los cuales se aplicaron las habilidades adquiridas como análisis exploratorio de datos EDA, análisis estadístico de datos, prueba de hipótesis, cálculo de métricas, implementación de una prueba A/B, probabilidades, pronósticos y tableros de visualización.

# Predicción de cancelación de clientes y segmentación de usuarios — Proyecto para Model Fitness
Descripción del proyecto:

Como parte del equipo de análisis de datos en Model Fitness, una cadena de gimnasios en proceso de transformación digital, desarrollé un modelo predictivo para identificar clientes con alto riesgo de cancelación y una segmentación de usuarios para diseñar estrategias personalizadas de retención. Este proyecto tuvo como objetivo principal reducir la tasa de rotación de clientes mediante un enfoque analítico.

## Objetivos del proyecto:

Predecir la probabilidad de cancelación de los clientes para el mes siguiente.

Identificar segmentos de usuarios según sus hábitos y características.

Detectar los factores clave que influyen en la pérdida de clientes.

Formular recomendaciones estratégicas para la retención basadas en análisis de datos.

## Análisis exploratorio de datos (EDA)
Se trabajó con datos de clientes, historial de visitas, servicios adicionales, tipo de contrato y datos sociodemográficos.

### Principales tareas:

Análisis descriptivo de características como edad, frecuencia de asistencia, duración del contrato y uso de servicios adicionales.

Comparación de métricas clave entre clientes que permanecieron y los que se dieron de baja.

Visualización de distribuciones y creación de una matriz de correlación para identificar relaciones entre variables.

## Modelado predictivo: clasificación de cancelación
Se desarrollaron y compararon dos modelos de clasificación:

Regresión logística

Bosque aleatorio (Random Forest)

### Resultados:

Ambos modelos fueron evaluados por precisión, recall y exactitud.

El modelo de bosque aleatorio ofreció mejores métricas de desempeño, siendo más robusto frente a variabilidad de datos.

## Segmentación de usuarios (Clustering)
Se llevó a cabo una segmentación de clientes mediante K-means (k=5), previa estandarización de las variables:

Análisis jerárquico con dendrogramas para estimar el número óptimo de clústeres.

Evaluación de diferencias entre grupos en características clave como frecuencia de visitas, uso de servicios, edad, tipo de contrato.

Cálculo de tasas de cancelación por clúster, identificando perfiles de alto y bajo riesgo.

## Hallazgos clave:
Los clientes con contratos más largos, participación en clases grupales y mayor gasto en servicios adicionales presentaron menores tasas de cancelación.

Aquellos con contratos mensuales, baja frecuencia de visitas y sin vínculos promocionales o cercanía geográfica fueron los más propensos a abandonar.

La variable “Lifetime” (meses como cliente) tuvo alta correlación negativa con la cancelación: a mayor antigüedad, mayor lealtad.

## Recomendaciones estratégicas:
Segmentación activa de clientes para campañas personalizadas según riesgo de cancelación.

Promoción de contratos de largo plazo con beneficios adicionales.

Fomento de clases grupales como herramienta de fidelización.

Ofertas personalizadas para clientes nuevos o inactivos, como descuentos en servicios adicionales o invitaciones a eventos.

## Herramientas utilizadas:

Python (pandas, numpy, matplotlib, seaborn, scikit-learn, scipy)

Jupyter Notebook

Algoritmos de machine learning supervisado y no supervisado

https://github.com/GuillermoTeran/Prediccion-de-cancelacion-de-clientes-y-segmentacion-de-usuarios-Proyecto-para-Model-Fitness



# Caso de Estudio: Dashboard de Tendencias de Videos en YouTube
Descripción del proyecto:

Como analista de videos publicitarios en la agencia Sterling & Draper, era responsable de detectar qué categorías de videos en YouTube marcaban tendencia para enfocar estrategias de mercadotecnia. Las consultas semanales sobre tendencias por parte de mis colegas motivaron la automatización de este proceso mediante la creación de un dashboard interactivo en Tableau Public.

## Objetivos del Proyecto
Identificar categorías de videos en tendencia cada semana.

Visualizar la distribución de estas categorías por país.

Detectar qué contenidos fueron particularmente populares en los Estados Unidos.

Crear un dashboard intuitivo y dinámico para uso diario por parte del equipo de planificación de marketing.

## Fuente de Datos
Archivo: trending_by_time.csv

Ubicación: Base de datos youtube

Estructura de la tabla trending_by_time:

record_id: ID único del registro

region: país o región

trending_date: fecha del evento

category_title: categoría del video

videos_count: número de videos en tendencia

## Frecuencia de Actualización
Datos actualizados cada 24 horas, a la medianoche UTC.

## Usuarios del Dashboard
Usuarios objetivo: gerentes de planificación de campañas publicitarias

Frecuencia de uso esperada: al menos una vez al día

## Contenido y Visualizaciones del Dashboard
Título y descripción del dashboard	Filtro de fecha y hora	Filtro de país
Gráfico "Historial de tendencias": tendencias de videos divididas por tiempo y categoría (valores absolutos, gráfico de área)	✅ Se puede ajustar el período de análisis por fecha/hora	✅ El filtro afecta todos los gráficos
Gráfico "Historial de tendencias" (%): proporción de categorías por fecha (gráfico de área con porcentajes)	✅	✅
Gráfico "Tendencias por país": distribución de tendencias por país (gráfico de pastel con valores relativos)	✅	Aplicable solo si se seleccionan múltiples países
Tabla "Tendencias por país y categoría": categorías y países cruzados, resaltado por valores absolutos	✅	✅ (Celdas resaltadas según intensidad de valores)

## Herramientas Utilizadas
Visualización y dashboard: Tableau Public

Procesamiento de datos previos: Python (Pandas)

Base de datos: PostgreSQL (simulada para el caso local)

Compartición: Publicado en Tableau Public con acceso abierto

## Análisis Realizado con el Dashboard
¿Qué categorías estuvieron más en tendencia?

Las categorías de música y entretenimiento dominaron durante la mayoría de las semanas.

¿Cómo se distribuyeron por país?

En países como India y México, música representó más del 60% de los videos en tendencia.

En Estados Unidos, la categoría Noticias y Política tuvo un aumento notable.

¿Qué categorías fueron especialmente populares en EE. UU.?

Noticias y Política, seguido de Entretenimiento.

En contraste, en Latinoamérica y Asia, Música fue más predominante.

## Insights Clave
Las categorías más virales varían significativamente según la región.

Hay patrones estacionales en ciertas categorías (e.g., más noticias en épocas electorales).

Estados Unidos presenta una diversidad mayor de categorías en comparación con otros países.

## Resultados y Beneficios
Automatización del análisis semanal, eliminando consultas repetitivas.

El dashboard permite segmentar tendencias en tiempo real.

Mejora en la capacidad de planificación de campañas publicitarias orientadas por datos.
https://public.tableau.com/views/Libro1_17212954380800/Dashboard1?:language=es-ES&publish=yes&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link 

https://github.com/GuillermoTeran/-Caso-de-Estudio-Dashboard-de-Tendencias-de-Videos-en-YouTube



# Análisis de comportamiento de usuario y test A/A/B en una app de productos alimenticios
Descripción del proyecto:

En este proyecto, trabajé como analista de datos para una startup dedicada a la venta de productos alimenticios a través de su aplicación móvil. El objetivo principal fue comprender cómo los usuarios interactúan con la aplicación y cómo las decisiones de diseño pueden impactar sus comportamientos, específicamente en relación con la conversión de ventas.

## Objetivos principales:
Analizar el embudo de conversión para detectar puntos de fricción en el recorrido del usuario.

Evaluar un experimento A/A/B diseñado para medir el impacto de un cambio en la tipografía de la interfaz.

Validar la correcta segmentación de los grupos de prueba.

Proporcionar recomendaciones basadas en datos para mejorar la experiencia del usuario.

## Datos utilizados:
Dataset: logs_exp_us.csv

Cada registro representa un evento de usuario dentro de la aplicación.

Campos principales:

event_name: tipo de acción realizada por el usuario.

device_id_hash: identificador único del usuario.

event_timestamp: marca de tiempo del evento.

exp_id: grupo experimental (246 y 247 son control; 248 es prueba).

## Paso 1: Lectura y preparación de datos
Se cargaron y revisaron los datos.

Se renombraron columnas para facilitar la lectura.

Se transformaron los tipos de datos y se extrajo la fecha del timestamp.

Se identificaron valores faltantes y se validó su impacto.

## Paso 2: Exploración de datos
Se identificaron 5 eventos y 7551 usuarios únicos.

Promedio de eventos por usuario: 32.28

El rango temporal cubierto fue de 2019-07-25 a 2019-08-07

Al trazar la distribución de eventos por fecha, se observó que los primeros días tenían registros incompletos.

Se estableció una fecha de corte para asegurar integridad de los datos, minimizando el sesgo.

## Paso 3: Análisis del embudo de conversión
Se identificaron los eventos más comunes y su orden lógico en el flujo de usuario.
Ejemplo:

App Launch

Product View

Add to Cart

Checkout

Payment Success

Se calculó la proporción de usuarios que pasaron de una etapa a la siguiente.

Etapa con mayor pérdida: entre Add to Cart y Checkout.

Solo un 47.68% de los usuarios completó el recorrido completo hasta el pago.

Estos resultados destacan áreas críticas para mejoras en la experiencia de usuario o incentivos de conversión.

## Paso 4: Evaluación del test A/A/B
### Validación del test A/A
Se compararon los grupos 246 y 247 (ambos con tipografía original).

Para cada evento:

Se calcularon proporciones de usuarios que realizaron la acción.

Se aplicó una prueba de hipótesis (proporciones) para validar si las diferencias eran significativas.

Resultado: No se detectaron diferencias significativas → segmentación válida.

### Análisis del grupo B (fuente nueva)
Se repitió el análisis para el grupo 248 (fuente nueva), comparándolo con:

Cada grupo de control individualmente.

Ambos grupos de control combinados.

Eventos clave analizados:

Visualización de productos

Agregar al carrito

Finalización de compra

Resultados:

Para algunos eventos, se observó una ligera caída en la interacción con la nueva tipografía.

Sin embargo, la mayoría de las diferencias no fueron estadísticamente significativas.

## Paso 5: Prueba de hipótesis y corrección por comparaciones múltiples
Hipótesis nula (H₀): no hay diferencia entre los grupos.

Hipótesis alternativa (H₁): existe una diferencia significativa entre los grupos.

Nivel de significancia original: α = 0.05.

Se realizaron múltiples pruebas (≈ N pruebas).

Se aplicó la corrección de Bonferroni para controlar el error tipo I:

Nuevo α ajustado: α/N.

Tras el ajuste, las diferencias dejaron de ser significativas → no se pudo concluir que la tipografía nueva afecte el comportamiento del usuario.

## Conclusiones:
El embudo reveló puntos de abandono importantes en la etapa previa al checkout, lo que indica una oportunidad clara de mejora en la conversión.

El experimento A/A/B mostró que:

Los grupos de control fueron consistentes.

El grupo con tipografía nueva no mostró mejoras significativas.

Recomendación: Postergar o repensar el cambio tipográfico, ya que no aporta un beneficio claro y puede introducir riesgo innecesario.

## Herramientas utilizadas:
Python (pandas, matplotlib, seaborn, scipy, statsmodels)

Jupyter Notebook

Estadística inferencial (prueba de proporciones, corrección por comparaciones múltiples)

## Impacto del análisis:
Este análisis proporcionó evidencia crítica para decisiones de producto, ayudando a la empresa a evitar cambios visuales que no aportaban valor al usuario. Asimismo, el embudo permitió identificar cuellos de botella clave en la experiencia de compra, facilitando decisiones más informadas para aumentar la conversión.

https://github.com/GuillermoTeran/Analisis-de-comportamiento-de-usuario-y-test-A-A-B-en-una-app-de-productos-alimenticios



# Caso de Estudio SQL: Análisis del Comportamiento de Lectores Durante la Pandemia
Descripción del proyecto:

Durante la pandemia por COVID-19, el cambio en los hábitos sociales impulsó el crecimiento del consumo de libros y el desarrollo de nuevas plataformas para lectores. En este proyecto, trabajé con una base de datos relacional de una startup del sector editorial que busca lanzar un nuevo producto digital para lectores y lectoras. A partir de los datos disponibles, el objetivo era identificar oportunidades de valor para esta propuesta.

## Objetivos del Proyecto
Explorar la base de datos para entender el comportamiento de lectura y calificación.

Ejecutar consultas SQL para extraer métricas clave sobre:

Publicaciones recientes

Participación de usuarios

Rendimiento de autores y editoriales

Generar insights que fundamenten decisiones de producto y estrategia.

## Descripción de la Base de Datos
La base de datos contenía cinco tablas principales:

Tabla	Contenido
books	Información sobre libros: título, fecha, páginas
authors	Autores/as
publishers	Editoriales
ratings	Calificaciones numéricas de los usuarios
reviews	Reseñas textuales de los usuarios

## Relaciones:

Cada libro está relacionado con un autor y una editorial.

Las calificaciones y reseñas están vinculadas a los libros mediante book_id.

## Tecnologías Utilizadas
SQL (PostgreSQL)

Jupyter Notebook

Python (Pandas solo para impresión de resultados)

## Consultas Realizadas y Hallazgos Clave
1. Libros publicados después del 1 de enero del 2000
Resultado: Se identificó un volumen creciente de publicaciones tras el año 2000, lo cual respalda la idea de que la plataforma puede enfocarse en títulos modernos.

2. Calificaciones promedio y número de reseñas por libro
Se agruparon datos por book_id para calcular el promedio de calificación y la cantidad de reseñas.

Resultado: Algunos títulos altamente calificados no eran los más populares en número de reseñas, lo que sugiere oportunidades para destacar “joyas ocultas”.

3. Editorial con más libros de más de 50 páginas
Filtro por libros con más de 50 páginas para excluir publicaciones cortas o folletos.

Resultado: Se identificó una editorial líder en publicaciones extensas, útil para alianzas comerciales o recomendaciones editoriales dentro de la app.

4. Autor con la mejor calificación promedio (mínimo 50 ratings)
Utilicé una subconsulta para filtrar libros con suficiente volumen de calificaciones.

Resultado: Se obtuvo un ranking confiable de autores con buena recepción crítica, ideal para destacar contenido de calidad.

5. Reseñas promedio por usuarios con más de 50 calificaciones
Se analizó el comportamiento de los usuarios más activos.

Resultado: Estos usuarios escriben más reseñas de texto que el promedio, por lo que podrían ser aprovechados como embajadores de la comunidad o creadores de contenido.

## Conclusiones Generales
La combinación de datos de reseñas, calificaciones y metadatos editoriales permite desarrollar estrategias efectivas para personalización de contenido.

Existen autores y libros con alto potencial de recomendación que aún no son ampliamente reconocidos.

Los usuarios más comprometidos generan un volumen significativo de contenido valioso (reseñas), y podrían ser clave para la fidelización.

## Valor para el Producto
Segmentación de contenido según editoriales líderes o autores de alto rendimiento.

Enfoque en usuarios activos para campañas de participación.

Curación de contenido basada en calidad percibida más que en volumen de calificaciones.

https://github.com/GuillermoTeran/Caso-de-Estudio-SQL-Analisis-del-Comportamiento-de-Lectores-Durante-la-Pandemia



# Caso de Estudio: Detección de Operadores Ineficaces en un Servicio de Telefonía Virtual
Descripción del proyecto:

La empresa de telefonía virtual CallMeMaybe buscaba identificar operadores con bajo rendimiento para optimizar la atención al cliente. Como analista de datos, lideré un proyecto de análisis exploratorio para encontrar operadores ineficaces basándome en múltiples indicadores operativos.

## Objetivos del Proyecto
Realizar un análisis exploratorio de datos (EDA) para comprender el comportamiento operativo.

Establecer métricas para determinar la ineficacia operativa.

Identificar operadores con bajo rendimiento.

Validar hipótesis mediante pruebas estadísticas.

## Fuentes y Estructura de Datos
1. telecom_dataset_us.csv

Información sobre llamadas entrantes, salientes e internas.

Variables clave:

operator_id, calls_count, is_missed_call, call_duration, total_call_duration, internal, direction

2. telecom_clients_us.csv

Información de clientes:

user_id, tariff_plan, date_start

## Criterios para Evaluar la Ineficacia
Alta proporción de llamadas entrantes perdidas (especialmente externas).

Tiempo de espera elevado (diferencia entre total_call_duration y call_duration).

Baja cantidad de llamadas salientes, para operadores cuya función incluye realizarlas.

Filtrado y agrupamiento por operador para comparar el rendimiento relativo.

## Herramientas Utilizadas
Python (Pandas, Seaborn, SciPy)

Jupyter Notebook

Análisis de hipótesis: Prueba t y prueba U de Mann-Whitney

Visualización: Matplotlib, Seaborn

## Análisis Exploratorio y Resultados
Operadores con más del 40% de llamadas perdidas fueron considerados críticos.

Se detectó que algunos operadores tenían un promedio de espera > 40% del total de la duración de llamada.

Se identificaron operadores asignados a tareas salientes con una tasa muy baja de llamadas realizadas.

## Conclusiones y Recomendaciones
Se listaron los operadores más ineficaces para revisión por Recursos Humanos y Supervisión.

Se recomendó ajustar la asignación de operadores en función del tráfico de llamadas.

Se propuso desarrollar alertas automáticas para detectar operadores ineficaces en tiempo real.


## Caso de Estudio: Evaluación de una Prueba A/B para un Sistema de Recomendaciones
Descripción del proyecto:

Una tienda en línea internacional realizó una prueba A/B para evaluar un nuevo sistema de recomendaciones. La tarea fue retomada tras ser abandonada por el equipo anterior. Mi objetivo fue validar la calidad del experimento y analizar sus resultados.

## Objetivos del Estudio
Validar el diseño y ejecución de la prueba A/B.

Analizar conversiones en cada etapa del embudo (product_page → product_card → purchase).

Determinar si hubo mejoras significativas en la conversión gracias al nuevo sistema.

## Datos Utilizados
Dataset	Descripción
final_ab_new_users_upd_us.csv	Nuevos usuarios y sus características
final_ab_events_upd_us.csv	Eventos de interacción de los usuarios
final_ab_participants_upd_us.csv	Participantes y su grupo de prueba
ab_project_marketing_events_us.csv	Calendario de campañas de marketing

## Herramientas Utilizadas
Python (Pandas, NumPy, SciPy)

Gráficos: Plotly, Seaborn

Pruebas estadísticas: Z-test para comparación de proporciones

Gestión del experimento: Verificación de superposición de usuarios, distribución de eventos por día

## Validaciones Previas al Análisis
Conversión de tipos y manejo de valores nulos.

Verificación de que no existieran usuarios en ambos grupos.

Confirmación de que la distribución de eventos por día y por usuario fuera similar entre grupos.

Revisión de eventos de marketing concurrentes que pudieran sesgar los resultados.

## Resultados del Análisis
Se encontró una mejora del 12% en la tasa de visitas a la página del producto en el grupo B.

Las tasas de product_card y purchase también mejoraron, pero solo alcanzaron significancia estadística en la primera etapa (product_page).

El grupo B mostró una mayor retención, pero se recomendó más tiempo de observación para validar compras.

## Conclusiones y Recomendaciones
El nuevo sistema de recomendaciones mejora la atracción inicial del usuario.

Se recomienda iterar sobre el embudo de compras para mejorar conversión en las etapas posteriores.

La prueba A/B fue válida, aunque se sugiere una muestra más grande para confirmar efectos en compras.

https://github.com/GuillermoTeran/Caso-de-Estudio-Deteccion-de-Operadores-Ineficaces-en-un-Servicio-de-Telefonia-Virtual



# Análisis de datos para Zuber: Comportamiento de viajes compartidos en Chicago
Descripción del proyecto:

Como analista de datos para Zuber, una nueva empresa de viajes compartidos en Chicago, me encargué de identificar patrones clave en los datos de transporte urbano. El objetivo fue comprender mejor las preferencias de los pasajeros, el desempeño de los competidores y el impacto del clima en los viajes, con un enfoque particular en el mes de noviembre de 2017.

El análisis incluyó la integración de múltiples fuentes de datos, consultas SQL, visualización en Python y pruebas estadísticas.

## Objetivos del análisis:
Analizar el comportamiento de los competidores de Zuber en términos de volumen de viajes.

Identificar los barrios más populares para dejar pasajeros.

Investigar si el clima lluvioso afecta la duración de los viajes desde el centro de Chicago (Loop) hasta el Aeropuerto O'Hare.

Proveer conclusiones accionables para estrategias de mercado y operaciones.

## Paso 1: Análisis de clima en Chicago
Se recopiló información desde un recurso externo que contenía condiciones meteorológicas en Chicago durante noviembre de 2017. Este análisis fue clave para vincular el clima con el comportamiento de viaje, especialmente los días sábado.

## Paso 2: Análisis SQL
Consultas destacadas:

Número de viajes por empresa (15–16 nov): Identifiqué las empresas más activas, destacándose Flash Cab y Taxi Affiliation Services.

Viajes de empresas "Yellow" o "Blue" (1–7 nov): Analicé el comportamiento de marcas tradicionales.

Agrupación de empresas: Agrupé las empresas principales y clasifiqué al resto como "Other" para simplificar el análisis de participación en el mercado.

Resultado: Se evidenció una alta concentración del mercado en unas pocas compañías.

## Paso 3: Hipótesis sobre clima y duración de viajes
Pregunta clave:

¿Cambia la duración promedio de los viajes desde Loop hasta O’Hare en sábados lluviosos?

Pasos seguidos:

Clasifiqué el clima en dos categorías: "Bad" (lluvia/tormenta) y "Good".

Seleccioné solo los viajes entre Loop (neighborhood_id 50) y O'Hare (neighborhood_id 63) realizados los sábados.

Vinculé cada viaje con las condiciones meteorológicas correspondientes.

## Paso 4: Análisis exploratorio en Python
Trabajé con tres datasets exportados desde SQL:

1. Empresas de taxi (project_sql_result_01.csv):
Visualización del número de viajes por empresa.

Flash Cab lideró por amplio margen en volumen de viajes.

2. Barrios de destino (project_sql_result_04.csv):
Identifiqué los 10 barrios principales en términos de viajes finalizados.

Se observaron zonas céntricas y turísticas entre las más frecuentadas.

3. Duración de viajes y clima (project_sql_result_07.csv):
Dataset base para la prueba de hipótesis.

## Paso 5: Prueba de hipótesis con Python
Hipótesis formuladas:

H₀ (nula): La duración media de los viajes no cambia entre sábados con buen y mal clima.

H₁ (alternativa): La duración media de los viajes sí cambia entre sábados con buen y mal clima.

Método:

Prueba de hipótesis para dos muestras independientes (t-test).

Nivel de significancia α = 0.05.

Resultado:

El valor p fue mayor que 0.05, por lo tanto no se rechaza la hipótesis nula.

Conclusión: No se encontraron diferencias significativas en la duración de los viajes entre sábados lluviosos y no lluviosos.

## Conclusiones generales:
Zuber enfrenta fuerte competencia de empresas establecidas como Flash Cab.

Los patrones de destino muestran una alta concentración en barrios céntricos.

El clima lluvioso no parece afectar significativamente la duración de los viajes desde el Loop a O’Hare los sábados, aunque este patrón podría variar en otras fechas o trayectos.

## Herramientas utilizadas:
SQL (PostgreSQL): consultas complejas y agrupación de datos.

Python: pandas, matplotlib, seaborn, scipy.

Jupyter Notebook: para documentación y visualización del análisis.

## Impacto del proyecto:
Este análisis ayudó a Zuber a entender mejor la dinámica del mercado en Chicago, identificar áreas de alta demanda, y evaluar la influencia del clima sobre su operación. Los resultados permiten fundamentar decisiones estratégicas relacionadas con el posicionamiento, la competencia y la planificación operativa.

https://github.com/GuillermoTeran/Analisis-de-datos-para-Zuber-Comportamiento-de-viajes-compartidos-en-Chicago



# Análisis de  tarifas prepago para Megaline
Descripción del proyecto:

Como analista de datos para Megaline, un operador de telecomunicaciones, llevé a cabo un análisis de clientes para comparar el rendimiento de sus dos planes prepago: Surf y Ultimate. El objetivo principal era determinar cuál de los dos planes genera mayores ingresos, con el fin de optimizar la asignación del presupuesto publicitario.

Se trabajó con datos de 500 clientes, incluyendo sus patrones de uso durante 2018 en llamadas, mensajes y consumo de datos.

## Objetivos del análisis:
Preprocesar y limpiar múltiples fuentes de datos relacionadas con usuarios, llamadas, mensajes, internet y planes tarifarios.

Calcular los ingresos mensuales por cliente, teniendo en cuenta los límites incluidos en cada plan y los cargos adicionales.

Analizar el comportamiento de los usuarios de cada plan.

Utilizar pruebas estadísticas para determinar si existen diferencias significativas entre ingresos medios por plan y por región geográfica.

## Preparación y limpieza de datos
Archivos analizados:

megaline_users.csv: datos demográficos y plan de cada usuario.

megaline_calls.csv: duración y fechas de llamadas.

megaline_messages.csv: cantidad de SMS enviados.

megaline_internet.csv: uso mensual de internet.

megaline_plans.csv: detalles de cada tarifa (límites y costos).

Tareas realizadas:

Conversión de columnas a tipos de datos adecuados (datetime, int, str, etc.).

Cálculo del volumen mensual de minutos, SMS y datos por cliente.

Identificación y corrección de valores atípicos o inconsistentes.

Redondeo de llamadas y datos según las reglas de facturación de Megaline.

Cálculo de ingresos mensuales por cliente, sumando cargos adicionales y la cuota mensual.

## Análisis exploratorio
Se analizó el uso mensual promedio de cada servicio:

Minutos de llamadas: los usuarios del plan Surf superan más a menudo el límite, generando cargos adicionales.

Mensajes SMS: muy poco uso general; la mayoría de usuarios no supera los límites.

Datos móviles: plan Surf tiene un límite más bajo (15 GB), y muchos usuarios exceden ese umbral.

Se calcularon promedios, varianza y desviación estándar para cada tipo de uso por tarifa, y se representaron mediante histogramas.

## Pruebas estadísticas
Se plantearon y evaluaron las siguientes hipótesis:

### Hipótesis 1:
H₀ (nula): No hay diferencia significativa entre los ingresos promedio de los planes Surf y Ultimate.

H₁ (alternativa): Hay una diferencia significativa entre los ingresos promedio de los planes.

### Hipótesis 2:
H₀ (nula): No hay diferencia significativa en los ingresos promedio entre usuarios del área de NY-NJ y otras regiones.

H₁ (alternativa): Hay una diferencia significativa en los ingresos promedio entre regiones.

### Método aplicado:
Prueba de hipótesis de dos muestras independientes (t-test), con un valor de α = 0.05.

### Resultados:

Se encontró una diferencia estadísticamente significativa en los ingresos entre Surf y Ultimate, confirmando que uno de los planes es más rentable.

No se encontró evidencia suficiente para afirmar que los ingresos difieren significativamente entre NY-NJ y otras regiones.

## Conclusiones clave:
Aunque el plan Ultimate tiene una cuota mensual mayor, el plan Surf genera más cargos adicionales, especialmente en consumo de datos, lo que puede equilibrar o incluso superar los ingresos.

Existen patrones de uso distintos entre planes, lo que puede orientar decisiones sobre la promoción de cada tarifa.

El análisis estadístico proporciona bases sólidas para priorizar estrategias de marketing basadas en ingresos reales generados.

## Herramientas utilizadas:
Python: pandas, numpy, matplotlib, seaborn, scipy

Jupyter Notebook: para documentación y presentación del análisis

Técnicas de EDA, ingeniería de características, limpieza de datos y análisis estadístico

## Impacto del proyecto:
Este análisis ayudó a Megaline a entender qué tarifa maximiza los ingresos en función del comportamiento real de sus clientes, permitiendo una mejor asignación del presupuesto de publicidad y el diseño de estrategias personalizadas de adquisición y retención.

https://github.com/GuillermoTeran/Analisis-de-tarifas-prepago---Proyecto-Megaline



# Análisis de ventas de videojuegos y detección de patrones de éxito — Proyecto Ice Games
 Descripción del proyecto:

Trabajé en el análisis de un amplio conjunto de datos proporcionado por Ice, una tienda online de videojuegos con presencia global. El objetivo principal fue identificar patrones que determinen si un videojuego puede considerarse exitoso, con el fin de detectar proyectos prometedores y optimizar campañas de marketing para el año 2017.

## Objetivos principales:

Analizar datos históricos de ventas de videojuegos (hasta 2016).

Explorar variables como géneros, plataformas, reseñas de usuarios y expertos, y clasificaciones ESRB.

Determinar las plataformas y géneros más rentables por región.

Identificar factores que influyen significativamente en el éxito comercial de un videojuego.

Formular y validar hipótesis estadísticas sobre preferencias de usuarios.

## Responsabilidades y tareas clave:

### Preparación y limpieza de datos

Conversión de nombres de columnas a formato estándar (minúsculas).

Conversión y validación de tipos de datos apropiados.

Tratamiento de valores ausentes (análisis de causas, decisiones de imputación o exclusión).

Manejo de valores no definidos como "TBD".

Cálculo de ventas globales agregadas por juego.

### Análisis exploratorio y visualización

Evaluación de tendencias anuales en lanzamientos y ventas.

Identificación de plataformas líderes y en declive.

Análisis de vida útil de plataformas y su impacto en ventas.

Evaluación de correlación entre reseñas (usuarios y expertos) y volumen de ventas.

Análisis de géneros por rentabilidad y frecuencia de aparición.

### Segmentación regional

Perfil de usuario por región (Norteamérica, Europa y Japón).

Identificación de plataformas y géneros favoritos por zona geográfica.

Evaluación del impacto de las clasificaciones ESRB en las decisiones de compra.

### Validación de hipótesis

Prueba de hipótesis sobre las calificaciones medias de usuarios para plataformas (Xbox One vs. PC) y géneros (Acción vs. Deportes).

Aplicación de pruebas estadísticas (por ejemplo, t-test) con justificación del umbral alfa y criterios de decisión.

## Herramientas utilizadas:

Python (pandas, numpy, matplotlib, seaborn, scipy)

Jupyter Notebook

Estadística inferencial

Visualización de datos

## Resultados destacados:

Identificación de plataformas emergentes con proyección de crecimiento para el año siguiente.

Correlación moderada entre buenas reseñas y mayores ventas, más significativa en ciertas plataformas.

Preferencias regionales bien definidas que permiten segmentar campañas publicitarias con mayor precisión.

Recomendaciones estratégicas para inversión en géneros y plataformas específicas.

https://github.com/GuillermoTeran/Analisis-de-ventas-de-videojuegos-y-deteccion-de-patrones-de-exito-Proyecto-Ice-Games



# Priorización de hipótesis y análisis de prueba A/B para optimización de ingresos — Proyecto de E-commerce
Descripción del proyecto:

Como Analista de Datos en una gran tienda online, participé en un proyecto estratégico en conjunto con el departamento de marketing para identificar formas de aumentar los ingresos del sitio. El proyecto se dividió en dos fases: priorización de hipótesis mediante frameworks de negocio y análisis estadístico de una prueba A/B real.

## Objetivos principales:

Priorizar hipótesis de negocio para maximizar impacto y eficiencia en la implementación.

Ejecutar y analizar una prueba A/B para evaluar la efectividad de posibles mejoras.

Detectar anomalías, validar hipótesis estadísticas y tomar decisiones fundamentadas.

## Fase 1: Priorización de hipótesis

Se trabajó con un conjunto de nueve hipótesis que buscaban mejorar métricas clave del negocio (conversiones, ingresos, experiencia del usuario).

## T#areas realizadas:

Aplicación de los frameworks ICE (Impact, Confidence, Effort) y RICE (Reach, Impact, Confidence, Effort).

Cálculo de puntajes y ordenamiento de hipótesis según cada método.

Comparación y análisis crítico de la diferencia en las prioridades obtenidas por ICE y RICE, destacando cómo el alcance (Reach) puede cambiar la perspectiva de valor de una hipótesis.

## Fase 2: Análisis del test A/B

Utilizando los datos de comportamiento de usuarios, ingresos y visitas para los grupos de prueba A y B, se realizó un análisis detallado de la prueba A/B.

## Análisis exploratorio y estadístico:

Visualización del ingreso acumulado y tamaño promedio de pedido por grupo.

Análisis de la diferencia relativa acumulada en métricas clave (ingresos, conversiones).

Cálculo y visualización de tasas de conversión diarias.

Identificación de valores atípicos en número de pedidos y monto de pedidos por usuario mediante percentiles (95 y 99).

Evaluación del impacto de anomalías en los resultados generales.

## Pruebas estadísticas realizadas:

Comparación de tasas de conversión y tamaños promedio de pedido entre los grupos A y B, tanto con datos brutos como con datos filtrados (excluyendo outliers).

Uso de pruebas de hipótesis (Mann-Whitney U test) para determinar la significancia estadística de las diferencias observadas.

## Herramientas utilizadas:

Python (pandas, numpy, scipy, matplotlib, seaborn)

Jupyter Notebook

Análisis estadístico y visualización de datos

## Resultados clave:

El grupo B mostró inicialmente métricas superiores, pero estas diferencias no fueron consistentemente significativas tras eliminar valores atípicos.

La decisión final fue detener la prueba y concluir que no hay diferencia estadísticamente significativa entre los grupos A y B.

La priorización con RICE reveló oportunidades más eficientes que con ICE, permitiendo una mejor asignación de recursos para futuras pruebas.

https://github.com/GuillermoTeran/Priorizacion-de-hipotesis-y-analisis-de-prueba-A-B-para-optimizacion-de-ingresos---Proyecto-de-Ecome



# Análisis de comportamiento de compra de clientes — Proyecto Instacart
Descripción del proyecto:

Este proyecto consistió en el análisis de datos de Instacart, una plataforma de entrega de comestibles en línea. Utilizando un conjunto de datos real modificado para fines educativos, el objetivo fue explorar los hábitos de compra de los clientes, limpiar los datos y generar visualizaciones que comuniquen los principales hallazgos.

## Objetivos del análisis:
Realizar un preprocesamiento completo del dataset, corrigiendo tipos de datos, valores ausentes y duplicados.

Analizar patrones de compra en función del día de la semana, la hora del día y la frecuencia de pedidos.

Identificar los productos más populares, reordenados y añadidos primero al carrito.

Comprender el comportamiento recurrente del cliente mediante métricas como la proporción de reorden y la cantidad de artículos por pedido.

## Preparación y limpieza de datos
Se trabajó con cinco archivos principales:

instacart_orders.csv

products.csv

order_products.csv

aisles.csv

departments.csv

### Procesamiento aplicado:

Conversión de columnas a tipos de datos apropiados (int, category, datetime).

Identificación y tratamiento de valores ausentes, especialmente en columnas como days_since_prior_order.

Eliminación de duplicados con criterios lógicos según ID de usuario y orden.

Documentación de decisiones tomadas para garantizar trazabilidad y reproducibilidad.

## Análisis exploratorio de datos (EDA)
### A. Análisis temporal de pedidos
La mayoría de los pedidos se realizan entre las 9:00 y 17:00 horas, con un pico a las 10:00.

El domingo y el lunes son los días más activos para hacer pedidos.

Se observó un patrón de recurrencia de pedidos cada 7 días, indicando hábitos de compra semanales.

### B. Comportamiento de los usuarios
Comparando miércoles y sábados, el sábado mostró una mayor dispersión de horas de pedido, con más actividad en la mañana.

La mayoría de los clientes realizan entre 4 y 10 pedidos en total.

Los 20 productos más pedidos incluyen frutas frescas, leche, bananas orgánicas y pan.

### C. Hábitos de reorden y carrito
El número promedio de artículos por pedido es de aproximadamente 10 a 12 productos.

Los productos más comúnmente reordenados incluyen artículos de consumo frecuente como bananas, leche y huevos.

Se calculó la proporción de reorden por producto, destacando artículos con tasas de recompra superiores al 70%.

Se identificaron los productos más frecuentemente añadidos como el primer artículo al carrito, lo cual puede reflejar prioridades de los usuarios.

## Visualizaciones generadas:
Histogramas comparativos por hora y día de la semana.

Gráficos de barras para productos más populares y más reordenados.

Diagramas de densidad para distribución de pedidos por cliente.

Gráficos de dispersión y tablas ordenadas para análisis de reorden.

Todas las visualizaciones incluyeron:

✅ Títulos claros
✅ Ejes etiquetados
✅ Leyendas cuando fue necesario
✅ plt.show() para correcta visualización en Jupyter Notebook

## Conclusiones clave:
Los hábitos de compra siguen una estructura semanal y horaria muy marcada, útil para optimizar operaciones logísticas y campañas publicitarias.

Existen productos con alto potencial de fidelización y recurrencia que pueden formar parte de promociones o suscripciones.

Los datos permiten segmentar a los clientes según frecuencia y tipo de productos, abriendo la puerta a recomendaciones personalizadas y mejoras en retención.

## Herramientas utilizadas:

Python (pandas, numpy, matplotlib, seaborn)

Jupyter Notebook

Técnicas de EDA, limpieza de datos, visualización y segmentación de clientes

https://github.com/GuillermoTeran/Analisis-de-comportamiento-de-compra-de-clientes-Proyecto-Instacart



# Análisis de eficiencia de marketing y comportamiento de clientes — Proyecto para Showz
Descripción del proyecto:

Como parte de mis prácticas en el departamento de analítica de Showz, una empresa de venta de entradas para eventos, realicé un estudio integral para optimizar los gastos de marketing y entender mejor el comportamiento de los usuarios en la plataforma. El objetivo principal fue evaluar el retorno de inversión de diferentes canales de adquisición, mejorar la segmentación de clientes y ofrecer recomendaciones de inversión con base en datos.

## Objetivos del análisis:

Investigar cómo los usuarios interactúan con la plataforma y cuándo se convierten en clientes.

Calcular métricas clave como CAC, LTV, y ROMI por fuente de adquisición.

Evaluar la rentabilidad del gasto en marketing digital en distintos dispositivos y canales.

Establecer una base para decisiones estratégicas de inversión en marketing.

## Preparación de los datos
Se integraron tres datasets principales:

Visitas al sitio (visits_log_us.csv)

Órdenes y compras (orders_log_us.csv)

Gastos de marketing (costs_us.csv)

Las tareas incluyeron:

Conversión de tipos de datos y normalización de fechas.

Cálculo de sesiones por usuario y su duración.

Unión de datasets mediante claves comunes para análisis multifuente.

## Análisis de comportamiento del cliente
Se analizaron métricas clave relacionadas con el uso de la plataforma:

Frecuencia de visitas diaria, semanal y mensual.

Duración promedio de sesión y retorno de usuarios.

Tiempos de conversión desde el primer acceso hasta la primera compra (Conversion 0d, 1d, etc.).

Tamaño promedio del pedido y comportamiento de compra por cohorte.

LTV (Valor del tiempo de vida del cliente) para distintos segmentos.

## Análisis de marketing y rentabilidad
Se calcularon y visualizaron métricas clave:

Costo total y por fuente de adquisición.

CAC (Costo de adquisición de cliente) por canal.

ROMI (Retorno sobre inversión en marketing) por canal y dispositivo.

Comparación del rendimiento de canales como orgánico, redes sociales, publicidad pagada, etc.

## Hallazgos clave:
Las fuentes orgánicas y de referidos presentaron el mejor ROMI gracias a su bajo CAC.

Las plataformas móviles generaron más sesiones, pero las conversiones fueron más altas en escritorio.

El tiempo medio de conversión fue menor en campañas con CTA directas, como email marketing.

Algunos canales tuvieron un alto costo con bajo retorno, lo que permitió sugerir su desinversión.

## Recomendaciones de inversión en marketing:
Concentrar presupuesto en canales con ROMI positivo, como búsqueda orgánica, referidos y campañas específicas de remarketing.

Reducir inversión en canales con bajo LTV y alto CAC, como ciertas campañas de display no segmentadas.

Personalizar campañas por dispositivo, priorizando escritorio para conversiones y móvil para generación de leads.

Implementar análisis de cohortes mensuales para monitorear la eficiencia de campañas nuevas.

## Herramientas utilizadas:

Python (pandas, numpy, matplotlib, seaborn)

Jupyter Notebook

Análisis cohortes, atribución de canales, KPIs de marketing (LTV, CAC, ROMI)

## Impacto del proyecto:
Este análisis sentó las bases para una asignación de presupuesto basada en datos en el equipo de marketing, ayudando a reducir el CAC promedio y aumentar el ROI general de campañas publicitarias.

https://github.com/GuillermoTeran/Analisis-de-eficiencia-de-marketing-y-comportamiento-de-clientes-Proyecto-para-Showz





