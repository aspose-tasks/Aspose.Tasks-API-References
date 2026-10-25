---
title: "Prj"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Representa las propiedades compatibles del objeto."
type: docs
weight: 216
url: /es/java/com.aspose.tasks/prj/
---

**Inheritance:**
java.lang.Object
```
public class Prj
```

Representa las propiedades compatibles del objeto [Project](../../com.aspose.tasks/project).
## Campos

| Campo | Descripción |
| --- | --- |
| [ACTUALS_IN_SYNC](#ACTUALS-IN-SYNC) | Determina si todos los trabajos reales se han sincronizado con el proyecto. |
| [ADMIN_PROJECT](#ADMIN-PROJECT) | Determina si un proyecto es un proyecto administrativo. |
| [ARE_EDITABLE_ACTUAL_COSTS](#ARE-EDITABLE-ACTUAL-COSTS) | Determina si los costos reales son editables. |
| [AUTHOR](#AUTHOR) | El autor de un proyecto. |
| [AUTOLINK](#AUTOLINK) | Determina si las tareas insertadas o movidas se enlazan automáticamente. |
| [AUTO_ADD_NEW_RESOURCES_AND_TASKS](#AUTO-ADD-NEW-RESOURCES-AND-TASKS) | Determina si los nuevos recursos o tareas se añaden automáticamente a un grupo de recursos o tareas. |
| [AUTO_CALCULATE_ASSIGNMENT_COSTS](#AUTO-CALCULATE-ASSIGNMENT-COSTS) | Determina si el costo de asignación y el costo restante deben calcularse automáticamente usando el trabajo de la asignación y las tarifas de los recursos. |
| [BASELINE_FOR_EARNED_VALUE](#BASELINE-FOR-EARNED-VALUE) | La línea base específica utilizada para calcular los valores de variación. |
| [CALENDAR](#CALENDAR) | El calendario del proyecto. |
| [CATEGORY](#CATEGORY) | La categoría de un proyecto. |
| [COMMENTS](#COMMENTS) | Comentarios del proyecto. |
| [COMPANY](#COMPANY) | La empresa donde se creó un proyecto. |
| [CREATION_DATE](#CREATION-DATE) | La fecha y hora en que se creó un proyecto. |
| [CRITICAL_SLACK_LIMIT](#CRITICAL-SLACK-LIMIT) | Las tareas se consideran críticas por MS Project si la holgura total es menor o igual a este número de días. |
| [CURRENCY_CODE](#CURRENCY-CODE) | El código de moneda de tres letras definido en ISO 4217. |
| [CURRENCY_DIGITS](#CURRENCY-DIGITS) | El número de dígitos después del símbolo decimal. |
| [CURRENCY_SYMBOL](#CURRENCY-SYMBOL) | El símbolo de moneda utilizado en un proyecto. |
| [CURRENCY_SYMBOL_POSITION](#CURRENCY-SYMBOL-POSITION) | La ubicación del símbolo de moneda. |
| [CURRENT_DATE](#CURRENT-DATE) | La fecha del sistema. |
| [CUSTOM_DATE_FORMAT](#CUSTOM-DATE-FORMAT) | Formato de fecha personalizado de la vista del proyecto. |
| [DATE_FORMAT](#DATE-FORMAT) | Formato de fecha de la vista del proyecto. |
| [DAYS_PER_MONTH](#DAYS-PER-MONTH) | El número de días por mes. |
| [DEFAULT_FINISH_TIME](#DEFAULT-FINISH-TIME) | La hora de finalización predeterminada de las tareas nuevas. |
| [DEFAULT_FIXED_COST_ACCRUAL](#DEFAULT-FIXED-COST-ACCRUAL) | El tipo predeterminado cuando se acumulan costos fijos. |
| [DEFAULT_OVERTIME_RATE](#DEFAULT-OVERTIME-RATE) | La tarifa de horas extra predeterminada para los recursos nuevos. |
| [DEFAULT_STANDARD_RATE](#DEFAULT-STANDARD-RATE) | La tarifa estándar predeterminada para los recursos nuevos. |
| [DEFAULT_START_TIME](#DEFAULT-START-TIME) | La hora de inicio predeterminada de las tareas nuevas. |
| [DEFAULT_TASK_EV_METHOD](#DEFAULT-TASK-EV-METHOD) | El método de valor ganado predeterminado para tareas. |
| [DEFAULT_TASK_TYPE](#DEFAULT-TASK-TYPE) | El tipo predeterminado de tareas nuevas. |
| [DURATION_FORMAT](#DURATION-FORMAT) | El formato para expresar la duración total. |
| [EARNED_VALUE_METHOD](#EARNED-VALUE-METHOD) | El método predeterminado para calcular el valor ganado. |
| [EXTENDED_CREATION_DATE](#EXTENDED-CREATION-DATE) | Fecha utilizada para cálculo e informes. |
| [FINISH_DATE](#FINISH-DATE) | La fecha de finalización de un proyecto. |
| [FISCAL_YEAR_START](#FISCAL-YEAR-START) | Determina si se utiliza la numeración del año fiscal. |
| [FY_START_DATE](#FY-START-DATE) | El mes en que comienza el año fiscal. |
| [GUID](#GUID) | El GUID del proyecto. |
| [HONOR_CONSTRAINTS](#HONOR-CONSTRAINTS) | Determina si las tareas respetan sus fechas de restricción. |
| [HYPERLINK_BASE](#HYPERLINK-BASE) | Base de hipervínculo del proyecto. |
| [INSERTED_PROJECTS_LIKE_SUMMARY](#INSERTED-PROJECTS-LIKE-SUMMARY) | Determina si las subtareas se calculan como tareas resumen. |
| [KEEP_TASK_ON_NEAREST_WORKING_TIME_WHEN_MADE_AUTO_SCHEDULED](#KEEP-TASK-ON-NEAREST-WORKING-TIME-WHEN-MADE-AUTO-SCHEDULED) | Determina si las tareas manuales deben mantenerse en el tiempo de trabajo más cercano cuando se convierten en programadas automáticamente. |
| [KEYWORDS](#KEYWORDS) | Palabras clave del proyecto. |
| [LAST_AUTHOR](#LAST-AUTHOR) | Último autor del proyecto. |
| [LAST_PRINTED](#LAST-PRINTED) | Última hora de impresión del proyecto. |
| [LAST_SAVED](#LAST-SAVED) | La fecha en que un proyecto se guardó por última vez. |
| [MANAGER](#MANAGER) | El responsable del proyecto. |
| [MICROSOFT_PROJECT_SERVER_URL](#MICROSOFT-PROJECT-SERVER-URL) | Determina si un proyecto fue creado por un usuario de Project Server en lugar de un usuario NT. |
| [MINUTES_PER_DAY](#MINUTES-PER-DAY) | El número de minutos por día. |
| [MINUTES_PER_WEEK](#MINUTES-PER-WEEK) | El número de minutos por semana. |
| [MOVE_COMPLETED_ENDS_BACK](#MOVE-COMPLETED-ENDS-BACK) | Determina si el final de las porciones completadas de tareas programadas para iniciar después de la fecha de estado pero que comenzaron antes debe retrocederse a la fecha de estado. |
| [MOVE_COMPLETED_ENDS_FORWARD](#MOVE-COMPLETED-ENDS-FORWARD) | Determina si el final de las porciones completadas de tareas programadas para haber finalizado antes de la fecha de estado pero que comenzaron después debe adelantarse a la fecha de estado. |
| [MOVE_REMAINING_STARTS_BACK](#MOVE-REMAINING-STARTS-BACK) | Determina si el inicio de las porciones restantes de tareas programadas para iniciar después de la fecha de estado pero que comenzaron antes debe retrocederse a la fecha de estado. |
| [MOVE_REMAINING_STARTS_FORWARD](#MOVE-REMAINING-STARTS-FORWARD) | Determina si el inicio de las porciones restantes de tareas programadas para haber comenzado después debe adelantarse a la fecha de estado. |
| [MULTIPLE_CRITICAL_PATHS](#MULTIPLE-CRITICAL-PATHS) | Determina si se calculan múltiples rutas críticas. |
| [NAME](#NAME) | El nombre del proyecto. |
| [NEW_TASKS_ARE_MANUAL](#NEW-TASKS-ARE-MANUAL) | Determina si las nuevas tareas se crean como manuales. |
| [NEW_TASKS_EFFORT_DRIVEN](#NEW-TASKS-EFFORT-DRIVEN) | Determina si las nuevas tareas están basadas en el esfuerzo. |
| [NEW_TASKS_ESTIMATED](#NEW-TASKS-ESTIMATED) | Determina si una duración estimada se muestra por defecto. |
| [NEW_TASK_START_DATE](#NEW-TASK-START-DATE) | El tipo de fecha de inicio predeterminada para nuevas tareas. |
| [PROJECT_EXTERNALLY_EDITED](#PROJECT-EXTERNALLY-EDITED) | Determina si el proyecto fue editado externamente. |
| [REMOVE_FILE_PROPERTIES](#REMOVE-FILE-PROPERTIES) | Determina si todas las propiedades del archivo se eliminarán al guardar. |
| [REVISION](#REVISION) | El número de veces que se guardó un proyecto. |
| [SAVE_VERSION](#SAVE-VERSION) | La versión de Microsoft Office Project con la que se guardó un archivo de proyecto. |
| [SCHEDULE_FROM_START](#SCHEDULE-FROM-START) | Determina si se debe calcular el cronograma del proyecto hacia adelante desde la fecha de inicio. |
| [SHOW_PROJECT_SUMMARY_TASK](#SHOW-PROJECT-SUMMARY-TASK) | Determina si se muestra la información resumida de todo un proyecto en una sola fila con su propia barra de tarea resumida en la parte superior de la vista de diagrama de Gantt. |
| [SPLITS_IN_PROGRESS_TASKS](#SPLITS-IN-PROGRESS-TASKS) | Determina si las tareas en curso pueden dividirse. |
| [SPREAD_ACTUAL_COST](#SPREAD-ACTUAL-COST) | Determina si los costos reales se distribuyen hasta la fecha de estado. |
| [SPREAD_PERCENT_COMPLETE](#SPREAD-PERCENT-COMPLETE) | Determina si el porcentaje de completado se distribuye hasta la fecha de estado. |
| [START_DATE](#START-DATE) | La fecha de inicio de un proyecto. |
| [STATUS_DATE](#STATUS-DATE) | la fecha de estado para mostrar el progreso o calcular los totales de valor ganado. |
| [SUBJECT](#SUBJECT) | El asunto del proyecto. |
| [TASK_UPDATES_RESOURCE](#TASK-UPDATES-RESOURCE) | Determina si las actualizaciones de tareas actualizan los recursos. |
| [TEMPLATE](#TEMPLATE) | Plantilla del proyecto. |
| [TIMESCALE_FINISH](#TIMESCALE-FINISH) | La fecha en que la escala de tiempo en la vista termina. |
| [TIMESCALE_START](#TIMESCALE-START) | La fecha en que la escala de tiempo en la vista comienza. |
| [TITLE](#TITLE) | El título de un proyecto. |
| [UID](#UID) | El Id único de un proyecto. |
| [UPDATE_MANUALLY_SCHEDULED_TASKS_WHEN_EDITING_LINKS](#UPDATE-MANUALLY-SCHEDULED-TASKS-WHEN-EDITING-LINKS) | Determina si las tareas manuales deben actualizarse cuando se editan los enlaces. |
| [WEEK_START_DAY](#WEEK-START-DAY) | Primer día de la semana. |
| [WORK_FORMAT](#WORK-FORMAT) | El formato utilizado para mostrar la duración de la tarea. |
### ACTUALS_IN_SYNC {#ACTUALS-IN-SYNC}
```
public static final Key<NullableBool,Byte> ACTUALS_IN_SYNC
```


Determina si todos los trabajos reales se han sincronizado con el proyecto.

### ADMIN_PROJECT {#ADMIN-PROJECT}
```
public static final Key<NullableBool,Byte> ADMIN_PROJECT
```


Determina si un proyecto es un proyecto administrativo.

### ARE_EDITABLE_ACTUAL_COSTS {#ARE-EDITABLE-ACTUAL-COSTS}
```
public static final Key<NullableBool,Byte> ARE_EDITABLE_ACTUAL_COSTS
```


Determina si los costos reales son editables.

### AUTHOR {#AUTHOR}
```
public static final Key<String,Byte> AUTHOR
```


El autor de un proyecto.

### AUTOLINK {#AUTOLINK}
```
public static final Key<NullableBool,Byte> AUTOLINK
```


Determina si las tareas insertadas o movidas se enlazan automáticamente.

### AUTO_ADD_NEW_RESOURCES_AND_TASKS {#AUTO-ADD-NEW-RESOURCES-AND-TASKS}
```
public static final Key<NullableBool,Byte> AUTO_ADD_NEW_RESOURCES_AND_TASKS
```


Determina si los nuevos recursos o tareas se añaden automáticamente a un grupo de recursos o tareas.

### AUTO_CALCULATE_ASSIGNMENT_COSTS {#AUTO-CALCULATE-ASSIGNMENT-COSTS}
```
public static final Key<Boolean,Byte> AUTO_CALCULATE_ASSIGNMENT_COSTS
```


Determina si el costo de asignación y el costo restante deben calcularse automáticamente usando el trabajo de la asignación y las tarifas de los recursos.

### BASELINE_FOR_EARNED_VALUE {#BASELINE-FOR-EARNED-VALUE}
```
public static final Key<Integer,Byte> BASELINE_FOR_EARNED_VALUE
```


La línea base específica utilizada para calcular los valores de variación.

### CALENDAR {#CALENDAR}
```
public static final Key<Calendar,Byte> CALENDAR
```


El calendario del proyecto.

### CATEGORY {#CATEGORY}
```
public static final Key<String,Byte> CATEGORY
```


La categoría de un proyecto.

### COMMENTS {#COMMENTS}
```
public static final Key<String,Byte> COMMENTS
```


Comentarios del proyecto.

### COMPANY {#COMPANY}
```
public static final Key<String,Byte> COMPANY
```


La empresa donde se creó un proyecto.

### CREATION_DATE {#CREATION-DATE}
```
public static final Key<Date,Byte> CREATION_DATE
```


La fecha y hora en que se creó un proyecto.

--------------------

Guardado en formato UTC en archivos mpp. Tipo java.util.Date.

### CRITICAL_SLACK_LIMIT {#CRITICAL-SLACK-LIMIT}
```
public static final Key<Integer,Byte> CRITICAL_SLACK_LIMIT
```


Las tareas se consideran críticas por MS Project si la holgura total es menor o igual a este número de días.

### CURRENCY_CODE {#CURRENCY-CODE}
```
public static final Key<String,Byte> CURRENCY_CODE
```


El código de tres letras de la moneda según la norma ISO 4217. Un ejemplo de valores válidos es "USD".

### CURRENCY_DIGITS {#CURRENCY-DIGITS}
```
public static final Key<Integer,Byte> CURRENCY_DIGITS
```


El número de dígitos después del símbolo decimal.

### CURRENCY_SYMBOL {#CURRENCY-SYMBOL}
```
public static final Key<String,Byte> CURRENCY_SYMBOL
```


El símbolo de moneda utilizado en un proyecto.

### CURRENCY_SYMBOL_POSITION {#CURRENCY-SYMBOL-POSITION}
```
public static final Key<Integer,Byte> CURRENCY_SYMBOL_POSITION
```


La ubicación del símbolo de moneda.

### CURRENT_DATE {#CURRENT-DATE}
```
public static final Key<Date,Byte> CURRENT_DATE
```


La fecha del sistema.

### CUSTOM_DATE_FORMAT {#CUSTOM-DATE-FORMAT}
```
public static final Key<String,Byte> CUSTOM_DATE_FORMAT
```


Formato de fecha personalizado de la vista del proyecto. Se utiliza para formatear fechas cuando la propiedad [DATE\_FORMAT](../../com.aspose.tasks/prj\#DATE-FORMAT) se establece en [DateFormat.Custom](../../com.aspose.tasks/dateformat\#Custom).

### DATE_FORMAT {#DATE-FORMAT}
```
public static final Key<Integer,Byte> DATE_FORMAT
```


Formato de fecha de la vista del proyecto.

### DAYS_PER_MONTH {#DAYS-PER-MONTH}
```
public static final Key<Integer,Byte> DAYS_PER_MONTH
```


El número de días por mes.

### DEFAULT_FINISH_TIME {#DEFAULT-FINISH-TIME}
```
public static final Key<Date,Byte> DEFAULT_FINISH_TIME
```


La hora de finalización predeterminada de las tareas nuevas.

### DEFAULT_FIXED_COST_ACCRUAL {#DEFAULT-FIXED-COST-ACCRUAL}
```
public static final Key<Integer,Byte> DEFAULT_FIXED_COST_ACCRUAL
```


El tipo predeterminado cuando se acumulan costos fijos.

### DEFAULT_OVERTIME_RATE {#DEFAULT-OVERTIME-RATE}
```
public static final Key<Double,Byte> DEFAULT_OVERTIME_RATE
```


La tarifa de horas extra predeterminada para los recursos nuevos.

### DEFAULT_STANDARD_RATE {#DEFAULT-STANDARD-RATE}
```
public static final Key<Double,Byte> DEFAULT_STANDARD_RATE
```


La tarifa estándar predeterminada para los recursos nuevos.

### DEFAULT_START_TIME {#DEFAULT-START-TIME}
```
public static final Key<Date,Byte> DEFAULT_START_TIME
```


La hora de inicio predeterminada de las tareas nuevas.

### DEFAULT_TASK_EV_METHOD {#DEFAULT-TASK-EV-METHOD}
```
public static final Key<Integer,Byte> DEFAULT_TASK_EV_METHOD
```


El método de valor ganado predeterminado para tareas.

### DEFAULT_TASK_TYPE {#DEFAULT-TASK-TYPE}
```
public static final Key<Integer,Byte> DEFAULT_TASK_TYPE
```


El tipo predeterminado de tareas nuevas.

### DURATION_FORMAT {#DURATION-FORMAT}
```
public static final Key<Byte,Byte> DURATION_FORMAT
```


El formato para expresar la duración total. Tipo `TimeUnitType`.

### EARNED_VALUE_METHOD {#EARNED-VALUE-METHOD}
```
public static final Key<Integer,Byte> EARNED_VALUE_METHOD
```


El método predeterminado para calcular el valor ganado.

### EXTENDED_CREATION_DATE {#EXTENDED-CREATION-DATE}
```
public static final Key<Date,Byte> EXTENDED_CREATION_DATE
```


Fecha utilizada para cálculo e informes.

### FINISH_DATE {#FINISH-DATE}
```
public static final Key<Date,Byte> FINISH_DATE
```


La fecha de finalización de un proyecto.

### FISCAL_YEAR_START {#FISCAL-YEAR-START}
```
public static final Key<NullableBool,Byte> FISCAL_YEAR_START
```


Determina si se utiliza la numeración del año fiscal.

### FY_START_DATE {#FY-START-DATE}
```
public static final Key<Integer,Byte> FY_START_DATE
```


El mes en que comienza el año fiscal.

### GUID {#GUID}
```
public static final Key<UUID,Byte> GUID
```


El GUID del proyecto.

### HONOR_CONSTRAINTS {#HONOR-CONSTRAINTS}
```
public static final Key<NullableBool,Byte> HONOR_CONSTRAINTS
```


Determina si las tareas respetan sus fechas de restricción.

### HYPERLINK_BASE {#HYPERLINK-BASE}
```
public static final Key<String,Byte> HYPERLINK_BASE
```


Base de hipervínculo del proyecto.

### INSERTED_PROJECTS_LIKE_SUMMARY {#INSERTED-PROJECTS-LIKE-SUMMARY}
```
public static final Key<NullableBool,Byte> INSERTED_PROJECTS_LIKE_SUMMARY
```


Determina si las subtareas se calculan como tareas resumen.

### KEEP_TASK_ON_NEAREST_WORKING_TIME_WHEN_MADE_AUTO_SCHEDULED {#KEEP-TASK-ON-NEAREST-WORKING-TIME-WHEN-MADE-AUTO-SCHEDULED}
```
public static final Key<NullableBool,Byte> KEEP_TASK_ON_NEAREST_WORKING_TIME_WHEN_MADE_AUTO_SCHEDULED
```


Determina si las tareas manuales deben mantenerse en el tiempo de trabajo más cercano cuando se convierten en programadas automáticamente.

### KEYWORDS {#KEYWORDS}
```
public static final Key<String,Byte> KEYWORDS
```


Palabras clave del proyecto.

### LAST_AUTHOR {#LAST-AUTHOR}
```
public static final Key<String,Byte> LAST_AUTHOR
```


Último autor del proyecto.

### LAST_PRINTED {#LAST-PRINTED}
```
public static final Key<Date,Byte> LAST_PRINTED
```


Última hora de impresión del proyecto.

--------------------

Guardado en formato UTC en archivos mpp. Tipo java.util.Date.

### LAST_SAVED {#LAST-SAVED}
```
public static final Key<Date,Byte> LAST_SAVED
```


La fecha en que un proyecto se guardó por última vez.

--------------------

Guardado en formato UTC en archivos mpp. Tipo java.util.Date.

### MANAGER {#MANAGER}
```
public static final Key<String,Byte> MANAGER
```


El responsable del proyecto.

### MICROSOFT_PROJECT_SERVER_URL {#MICROSOFT-PROJECT-SERVER-URL}
```
public static final Key<NullableBool,Byte> MICROSOFT_PROJECT_SERVER_URL
```


Determina si un proyecto fue creado por un usuario de Project Server en lugar de un usuario NT.

### MINUTES_PER_DAY {#MINUTES-PER-DAY}
```
public static final Key<Integer,Byte> MINUTES_PER_DAY
```


El número de minutos por día.

### MINUTES_PER_WEEK {#MINUTES-PER-WEEK}
```
public static final Key<Integer,Byte> MINUTES_PER_WEEK
```


El número de minutos por semana.

### MOVE_COMPLETED_ENDS_BACK {#MOVE-COMPLETED-ENDS-BACK}
```
public static final Key<NullableBool,Byte> MOVE_COMPLETED_ENDS_BACK
```


Determina si el final de las porciones completadas de tareas programadas para iniciar después de la fecha de estado pero que comenzaron antes debe retrocederse a la fecha de estado.

### MOVE_COMPLETED_ENDS_FORWARD {#MOVE-COMPLETED-ENDS-FORWARD}
```
public static final Key<NullableBool,Byte> MOVE_COMPLETED_ENDS_FORWARD
```


Determina si el final de las porciones completadas de tareas programadas para haber finalizado antes de la fecha de estado pero que comenzaron después debe adelantarse a la fecha de estado.

### MOVE_REMAINING_STARTS_BACK {#MOVE-REMAINING-STARTS-BACK}
```
public static final Key<NullableBool,Byte> MOVE_REMAINING_STARTS_BACK
```


Determina si el inicio de las porciones restantes de tareas programadas para iniciar después de la fecha de estado pero que comenzaron antes debe retrocederse a la fecha de estado.

### MOVE_REMAINING_STARTS_FORWARD {#MOVE-REMAINING-STARTS-FORWARD}
```
public static final Key<NullableBool,Byte> MOVE_REMAINING_STARTS_FORWARD
```


Determina si el inicio de las porciones restantes de tareas programadas para haber comenzado después debe adelantarse a la fecha de estado.

### MULTIPLE_CRITICAL_PATHS {#MULTIPLE-CRITICAL-PATHS}
```
public static final Key<NullableBool,Byte> MULTIPLE_CRITICAL_PATHS
```


Determina si se calculan múltiples rutas críticas.

### NAME {#NAME}
```
public static final Key<String,Byte> NAME
```


El nombre del proyecto.

### NEW_TASKS_ARE_MANUAL {#NEW-TASKS-ARE-MANUAL}
```
public static final Key<NullableBool,Byte> NEW_TASKS_ARE_MANUAL
```


Determina si las nuevas tareas se crean como manuales.

### NEW_TASKS_EFFORT_DRIVEN {#NEW-TASKS-EFFORT-DRIVEN}
```
public static final Key<NullableBool,Byte> NEW_TASKS_EFFORT_DRIVEN
```


Determina si las nuevas tareas están basadas en el esfuerzo.

### NEW_TASKS_ESTIMATED {#NEW-TASKS-ESTIMATED}
```
public static final Key<NullableBool,Byte> NEW_TASKS_ESTIMATED
```


Determina si una duración estimada se muestra por defecto.

### NEW_TASK_START_DATE {#NEW-TASK-START-DATE}
```
public static final Key<Integer,Byte> NEW_TASK_START_DATE
```


El tipo de fecha de inicio predeterminada para nuevas tareas.

### PROJECT_EXTERNALLY_EDITED {#PROJECT-EXTERNALLY-EDITED}
```
public static final Key<NullableBool,Byte> PROJECT_EXTERNALLY_EDITED
```


Determina si el proyecto fue editado externamente.

### REMOVE_FILE_PROPERTIES {#REMOVE-FILE-PROPERTIES}
```
public static final Key<NullableBool,Byte> REMOVE_FILE_PROPERTIES
```


Determina si todas las propiedades del archivo se eliminarán al guardar.

### REVISION {#REVISION}
```
public static final Key<Integer,Byte> REVISION
```


El número de veces que se guardó un proyecto.

### SAVE_VERSION {#SAVE-VERSION}
```
public static final Key<Integer,Byte> SAVE_VERSION
```


La versión de Microsoft Office Project con la que se guardó un archivo de proyecto.

### SCHEDULE_FROM_START {#SCHEDULE-FROM-START}
```
public static final Key<NullableBool,Byte> SCHEDULE_FROM_START
```


Determina si se debe calcular el cronograma del proyecto hacia adelante desde la fecha de inicio.

### SHOW_PROJECT_SUMMARY_TASK {#SHOW-PROJECT-SUMMARY-TASK}
```
public static final Key<Boolean,Byte> SHOW_PROJECT_SUMMARY_TASK
```


Determina si se muestra la información resumida de todo un proyecto en una sola fila con su propia barra de tarea resumida en la parte superior de la vista de diagrama de Gantt.

### SPLITS_IN_PROGRESS_TASKS {#SPLITS-IN-PROGRESS-TASKS}
```
public static final Key<NullableBool,Byte> SPLITS_IN_PROGRESS_TASKS
```


Determina si las tareas en curso pueden dividirse.

### SPREAD_ACTUAL_COST {#SPREAD-ACTUAL-COST}
```
public static final Key<NullableBool,Byte> SPREAD_ACTUAL_COST
```


Determina si los costos reales se distribuyen hasta la fecha de estado.

### SPREAD_PERCENT_COMPLETE {#SPREAD-PERCENT-COMPLETE}
```
public static final Key<NullableBool,Byte> SPREAD_PERCENT_COMPLETE
```


Determina si el porcentaje de completado se distribuye hasta la fecha de estado.

### START_DATE {#START-DATE}
```
public static final Key<Date,Byte> START_DATE
```


La fecha de inicio de un proyecto.

### STATUS_DATE {#STATUS-DATE}
```
public static final Key<Date,Byte> STATUS_DATE
```


la fecha de estado para mostrar el progreso o calcular los totales de valor ganado. La fecha de estado es la misma que la fecha actual (fecha de hoy) a menos que se especifique una fecha de estado diferente.

### SUBJECT {#SUBJECT}
```
public static final Key<String,Byte> SUBJECT
```


El asunto del proyecto.

### TASK_UPDATES_RESOURCE {#TASK-UPDATES-RESOURCE}
```
public static final Key<NullableBool,Byte> TASK_UPDATES_RESOURCE
```


Determina si las actualizaciones de tareas actualizan los recursos.

### TEMPLATE {#TEMPLATE}
```
public static final Key<String,Byte> TEMPLATE
```


Plantilla del proyecto.

### TIMESCALE_FINISH {#TIMESCALE-FINISH}
```
public static final Key<Date,Byte> TIMESCALE_FINISH
```


La fecha en que la escala de tiempo en la vista termina.

### TIMESCALE_START {#TIMESCALE-START}
```
public static final Key<Date,Byte> TIMESCALE_START
```


La fecha en que la escala de tiempo en la vista comienza.

### TITLE {#TITLE}
```
public static final Key<String,Byte> TITLE
```


El título de un proyecto.

### UID {#UID}
```
public static final Key<String,Byte> UID
```


El Id único de un proyecto.

### UPDATE_MANUALLY_SCHEDULED_TASKS_WHEN_EDITING_LINKS {#UPDATE-MANUALLY-SCHEDULED-TASKS-WHEN-EDITING-LINKS}
```
public static final Key<NullableBool,Byte> UPDATE_MANUALLY_SCHEDULED_TASKS_WHEN_EDITING_LINKS
```


Determina si las tareas manuales deben actualizarse cuando se editan los enlaces.

### WEEK_START_DAY {#WEEK-START-DAY}
```
public static final Key<Integer,Byte> WEEK_START_DAY
```


Primer día de la semana.

### WORK_FORMAT {#WORK-FORMAT}
```
public static final Key<Byte,Byte> WORK_FORMAT
```


El formato utilizado para mostrar la duración de la tarea.

