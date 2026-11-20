# Dashboard de Paros y Rendimiento (OEE)

## Descripción del proyecto

Proyecto de análisis de datos orientado al seguimiento del rendimiento operativo de una planta de producción mediante indicadores OEE (*Overall Equipment Effectiveness*).

El objetivo es identificar patrones de inactividad, analizar las principales causas de los tiempos de paro y proporcionar información que facilite la toma de decisiones y la optimización de los procesos productivos.

## Análisis y principales hallazgos

A partir del procesamiento y análisis de los datos, se identificaron los siguientes resultados:

### 1. Disponibilidad operativa

- **Disponibilidad general:** 62,14%.
- **Tiempo total de paro:** 23.730 horas.
- **Tiempo total de operación:** 38.950 horas.

Los resultados evidencian una proporción significativa de tiempo improductivo, lo que representa una oportunidad de mejora en la gestión operativa y la disponibilidad de los equipos.

### 2. Análisis de causas de paro

El análisis de Pareto permitió identificar tres causas principales que concentran aproximadamente el 80% del tiempo perdido:

| Causa de paro | Horas aproximadas |
|---|---:|
| Aprovisionamiento y aseo del puesto | 7.000 |
| Ajustes operativos | 5.000 |
| Limpieza por derrames | 5.000 |

Estos resultados permiten priorizar las acciones correctivas sobre los factores que tienen mayor impacto en la continuidad de la producción.

### 3. Rendimiento por línea de producción

- **Vinilos_4** registra el mayor volumen de horas operativas, con aproximadamente 13.800 horas.
- Se identifican incrementos en los tiempos de paro durante los meses de enero y diciembre en las diferentes líneas de producción.

Este comportamiento permite identificar períodos que requieren mayor seguimiento y planificación operativa.

## Propuestas de mejora

A partir de los hallazgos, se plantean las siguientes acciones:

1. **Optimización del aprovisionamiento:** establecer procedimientos de preparación anticipada de insumos y materiales para reducir las interrupciones por falta de recursos.
2. **Control de derrames:** identificar las causas de los derrames y establecer medidas preventivas que disminuyan los tiempos destinados a limpieza.
3. **Planificación del mantenimiento:** fortalecer las actividades de mantenimiento preventivo antes de los períodos de mayor incidencia de paros, especialmente durante los cierres e inicios de año.

## Arquitectura y herramientas utilizadas

El proyecto integra herramientas de gestión de bases de datos y visualización para construir una solución de análisis empresarial.

| Tecnología | Aplicación |
|---|---|
| PostgreSQL | Almacenamiento y gestión de datos |
| Power BI | Desarrollo del dashboard interactivo |
| DAX | Creación de medidas e indicadores |
| Modelo dimensional | Organización de los datos mediante un esquema estrella de 7 tablas |

## Componentes de la solución

- **Base de datos:** estructura relacional implementada en PostgreSQL bajo un modelo dimensional tipo estrella.
- **Dashboard interactivo:** visualización de indicadores y análisis mediante filtros por línea de producción, período y operario.
- **Indicadores:** medidas DAX para el cálculo de OEE, disponibilidad, horas de paro y Pareto acumulado.

## Objetivo del proyecto

Demostrar cómo la integración de bases de datos, análisis de datos y herramientas de Business Intelligence permite transformar registros operativos en información útil para identificar oportunidades de mejora y respaldar la toma de decisiones.
