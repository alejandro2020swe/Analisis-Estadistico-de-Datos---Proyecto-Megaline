# Análisis Estadístico de Datos - Proyecto Megaline

## Descripción del Proyecto

Este proyecto se enfoca en el análisis del comportamiento de los clientes de Megaline, un operador de telecomunicaciones que ofrece dos tarifas de prepago: Surf y Ultimate. El objetivo es determinar cuál de las dos tarifas genera más ingresos para la empresa, basándose en los datos de 500 clientes durante el año 2018.

## Descripción de las Tarifas

### Surf
- **Pago mensual:** $20
- **Incluye:** 500 minutos, 50 SMS, 15 GB de datos
- **Costos adicionales:**
  - Minuto adicional: $0.03
  - SMS adicional: $0.03
  - GB adicional: $10

### Ultimate
- **Pago mensual:** $70
- **Incluye:** 3000 minutos, 1000 SMS, 30 GB de datos
- **Costos adicionales:**
  - Minuto adicional: $0.01
  - SMS adicional: $0.01
  - GB adicional: $7

## Diccionario de Datos

### users.csv (Datos sobre los usuarios)
- `user_id`: Identificador único del usuario
- `first_name`: Nombre del usuario
- `last_name`: Apellido del usuario
- `age`: Edad del usuario
- `reg_date`: Fecha de suscripción
- `churn_date`: Fecha de finalización del servicio (nulo si sigue activo)
- `city`: Ciudad de residencia
- `plan`: Nombre de la tarifa

### calls.csv (Datos sobre las llamadas)
- `id`: Identificador único de la llamada
- `call_date`: Fecha de la llamada
- `duration`: Duración de la llamada en minutos
- `user_id`: Identificador del usuario que realizó la llamada

### messages.csv (Datos sobre los SMS)
- `id`: Identificador único del SMS
- `message_date`: Fecha del SMS
- `user_id`: Identificador del usuario que envió el SMS

### internet.csv (Datos sobre las sesiones web)
- `id`: Identificador único de la sesión
- `mb_used`: Volumen de datos utilizados durante la sesión (en MB)
- `session_date`: Fecha de la sesión web
- `user_id`: Identificador del usuario

### plans.csv (Datos sobre las tarifas)
- `plan_name`: Nombre de la tarifa
- `usd_monthly_fee`: Pago mensual en USD
- `minutes_included`: Minutos incluidos por mes
- `messages_included`: SMS incluidos por mes
- `mb_per_month_included`: Datos incluidos por mes (en MB)
- `usd_per_minute`: Costo por minuto adicional
- `usd_per_message`: Costo por SMS adicional
- `usd_per_gb`: Costo por GB adicional (1 GB = 1024 MB)

## Instrucciones para Completar el Proyecto

1. **Abrir y explorar los datos.**
2. **Preparar los datos:**
   - Convertir los datos a los tipos correctos.
   - Eliminar errores en los datos.
   - Calcular métricas por usuario: llamadas, SMS, datos y ingresos mensuales.
3. **Análisis de datos:**
   - Describir el comportamiento de los clientes.
   - Calcular estadísticas: media, varianza, desviación estándar.
   - Realizar pruebas de hipótesis sobre los ingresos generados por las tarifas.
4. **Escribir conclusiones.**

## Instrucciones del Proyecto

1. **Apertura y exploración de datos:**
   - Se abrieron los archivos de datos proporcionados y se realizó un análisis exploratorio inicial para entender la estructura y contenido de cada tabla.

2. **Preparación de los datos:**
   - Los datos fueron convertidos a los tipos de datos apropiados según su contexto (por ejemplo, fechas, enteros).
   - Se identificaron y eliminaron errores en los datos, como valores faltantes o duplicados.
   - Se calcularon las métricas relevantes para cada usuario, incluyendo:
     - Número total de llamadas y minutos utilizados por mes.
     - Cantidad de SMS enviados por mes.
     - Volumen de datos utilizados por mes.
     - Ingresos mensuales generados por cada usuario, considerando los costos adicionales por exceder los límites del plan.

3. **Análisis de datos:**
   - Se describió el comportamiento de los clientes en términos de minutos de llamada, SMS enviados y datos utilizados por mes.
   - Se calcularon estadísticas descriptivas como la media, la varianza y la desviación estándar para cada métrica.
   - Se generaron gráficos que muestran la distribución de las llamadas, SMS y uso de datos por los clientes de las dos tarifas.
   - Se identificaron las diferencias en el comportamiento entre los usuarios de las tarifas Surf y Ultimate.

4. **Pruebas de hipótesis:**
   - Se realizó una prueba de hipótesis para determinar si existe una diferencia significativa en el ingreso promedio generado por los usuarios de las tarifas Surf y Ultimate.
   - También se realizó una prueba de hipótesis para comparar los ingresos generados por los usuarios de Nueva York-Nueva Jersey con los de otras regiones.

5. **Conclusiones:**
   - Se redactaron conclusiones basadas en los análisis y pruebas estadísticas realizadas, destacando cuál tarifa es más rentable para Megaline y las diferencias en el comportamiento de los clientes según la región.
