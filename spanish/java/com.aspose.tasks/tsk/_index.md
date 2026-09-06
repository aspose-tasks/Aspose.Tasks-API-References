---
title: "Tsk"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Representa las propiedades de un objeto."
type: docs
weight: 328
url: /es/java/com.aspose.tasks/tsk/
---

**Inheritance:**
java.lang.Object
```
public class Tsk
```

Representa las propiedades del objeto [Task](../../com.aspose.tasks/task).
## Constructores

| Constructor | Descripción |
| --- | --- |
| [Tsk()](#Tsk--) |  |
## Campos

| Campo | Descripción |
| --- | --- |
| [ACTIVITY_ID](#ACTIVITY-ID) | Representa el campo de ID de actividad: el identificador único de una tarea utilizado por Primavera. |
| [ACTUAL_COST](#ACTUAL-COST) | Costos incurridos por el trabajo ya realizado por los recursos en sus tareas, junto con cualquier otro costo registrado asociado a la tarea. |
| [ACTUAL_DURATION](#ACTUAL-DURATION) | El período de tiempo de trabajo real para una tarea, basado en la duración programada y el trabajo restante actual o el porcentaje completado. |
| [ACTUAL_FINISH](#ACTUAL-FINISH) | La fecha en que se completó una tarea. |
| [ACTUAL_OVERTIME_COST](#ACTUAL-OVERTIME-COST) | Costos incurridos por trabajo extra ya realizado en tareas por los recursos asignados. |
| [ACTUAL_OVERTIME_WORK](#ACTUAL-OVERTIME-WORK) | La cantidad real de trabajo extra ya realizado por los recursos asignados a tareas. |
| [ACTUAL_OVERTIME_WORK_PROTECTED](#ACTUAL-OVERTIME-WORK-PROTECTED) | La duración durante la cual el trabajo extra real está protegido. |
| [ACTUAL_START](#ACTUAL-START) | La fecha y hora en que una tarea comenzó realmente. |
| [ACTUAL_WORK](#ACTUAL-WORK) | La cantidad de trabajo que ya se ha realizado por los recursos asignados a las tareas. |
| [ACTUAL_WORK_PROTECTED](#ACTUAL-WORK-PROTECTED) | La duración durante la cual el trabajo real está protegido. |
| [ACWP](#ACWP) | Costos incurridos por el trabajo ya realizado en una tarea, hasta la fecha de estado del proyecto o la fecha de hoy. |
| [BCWP](#BCWP) | El valor acumulado del porcentaje de completado de la tarea multiplicado por los costos de referencia basados en tiempo. |
| [BCWS](#BCWS) | Los costos de referencia acumulados basados en tiempo hasta la fecha de estado o la fecha de hoy. |
| [BUDGET_COST](#BUDGET-COST) | Costos presupuestarios para recursos de costo presupuestario. |
| [BUDGET_WORK](#BUDGET-WORK) | Trabajo presupuestado para recursos de trabajo y materiales. |
| [CALENDAR](#CALENDAR) | El calendario de la tarea. |
| [COMMITMENT_FINISH](#COMMITMENT-FINISH) | La fecha de finalización de una entrega. |
| [COMMITMENT_START](#COMMITMENT-START) | La fecha de inicio de una entrega. |
| [COMMITMENT_TYPE](#COMMITMENT-TYPE) | Determina si una tarea tiene una entrega asociada o una dependencia de una entrega asociada. |
| [CONSTRAINT_DATE](#CONSTRAINT-DATE) | La fecha específica asociada al tipo de restricción. |
| [CONSTRAINT_TYPE](#CONSTRAINT-TYPE) | Proporciona opciones para el tipo de restricción que se puede aplicar al programar una tarea. |
| [CONTACT](#CONTACT) | El nombre de la persona responsable de una tarea. |
| [COST](#COST) | El costo total programado o proyectado para una tarea basado en los costos ya incurridos por el trabajo realizado por los recursos asignados a las tareas, además de los costos planificados para el trabajo restante. |
| [COST_VARIANCE](#COST-VARIANCE) | La diferencia entre el costo de referencia y el costo total para una tarea, recurso o asignación. |
| [CREATED](#CREATED) | La fecha en que se creó una tarea. |
| [CV](#CV) | La diferencia entre el costo de referencia y el costo total para una tarea. |
| [DEADLINE](#DEADLINE) | Una fecha objetivo que indica cuándo debe completarse una tarea. |
| [DISPLAY_AS_SUMMARY](#DISPLAY-AS-SUMMARY) | Determina si la tarea debe mostrarse como una tarea resumen. |
| [DISPLAY_ON_TIMELINE](#DISPLAY-ON-TIMELINE) | Especifica si una tarea debe mostrarse en una vista de línea de tiempo. |
| [DURATION](#DURATION) | El período total de tiempo de trabajo activo para una tarea según se ingresó o según lo calcule Microsoft Project basado en la fecha de inicio, fecha de finalización, calendarios y otros factores de programación. |
| [DURATION_TEXT](#DURATION-TEXT) | Devuelve el texto de duración de la tarea. |
| [DURATION_VARIANCE](#DURATION-VARIANCE) | La diferencia entre la duración de referencia de una tarea y la duración total (estimación actual) de una tarea. |
| [EARLY_FINISH](#EARLY-FINISH) | La fecha más temprana en que una tarea podría finalizar, basada en las fechas de finalización temprana de las tareas predecesoras y sucesoras, otras restricciones y cualquier retraso de nivelación. |
| [EARLY_START](#EARLY-START) | La fecha más temprana en que una tarea podría comenzar, basada en las fechas de inicio temprano de las tareas predecesoras y sucesoras y otras restricciones. |
| [EARNED_VALUE_METHOD](#EARNED-VALUE-METHOD) | Determina si se debe usar el campo % Complete o Physical % Complete para calcular el costo presupuestado del trabajo realizado (BCWP). |
| [EXTERNAL_ID](#EXTERNAL-ID) | Si una tarea es una tarea externa, contiene el Id externo de la tarea. |
| [EXTERNAL_TASK_PROJECT](#EXTERNAL-TASK-PROJECT) | La ubicación de origen y el identificador de la tarea de una tarea externa. |
| [EXTERNAL_UID](#EXTERNAL-UID) | Contiene el identificador único de la tarea externa cuando la tarea es externa. |
| [FINISH](#FINISH) | La fecha de finalización programada de una tarea. |
| [FINISH_SLACK_TIME_SPAN](#FINISH-SLACK-TIME-SPAN) | La duración (en segundos) entre las fechas de Finalización Temprana y Finalización Tardía. |
| [FINISH_TEXT](#FINISH-TEXT) | Devuelve el texto de finalización de la tarea. |
| [FINISH_VARIANCE](#FINISH-VARIANCE) | El tiempo que representa la diferencia entre la fecha de finalización de referencia de una tarea o asignación y su fecha de finalización actual. |
| [FIXED_COST](#FIXED-COST) | Muestra cualquier gasto de tarea que no sea de recurso. |
| [FIXED_COST_ACCRUAL](#FIXED-COST-ACCRUAL) | Determina las opciones de cómo y cuándo se deben cargar o acumular los costos fijos al costo de una tarea. |
| [FREE_SLACK_TIME_SPAN](#FREE-SLACK-TIME-SPAN) | El tiempo (en segundos) que una tarea puede retrasarse sin retrasar ninguna tarea sucesora. |
| [GUID](#GUID) | Los códigos de identificación únicos generados para una tarea. |
| [HAS_OVERALLOCATED_RESOURCE](#HAS-OVERALLOCATED-RESOURCE) | Indica si la tarea tiene un recurso asignado que tiene más trabajo en tareas asignadas del que puede completarse dentro de la capacidad de trabajo normal. |
| [HIDE_BAR](#HIDE-BAR) | Determina si la barra Gantt de una tarea está oculta cuando se muestra en Microsoft Project. |
| [HYPERLINK](#HYPERLINK) | El título o texto explicativo de un hipervínculo asociado a una tarea. |
| [HYPERLINK_ADDRESS](#HYPERLINK-ADDRESS) | La dirección de un hipervínculo asociado a una tarea. |
| [HYPERLINK_SUB_ADDRESS](#HYPERLINK-SUB-ADDRESS) | La ubicación específica en un documento en un hipervínculo asociado a una tarea. |
| [ID](#ID) | El identificador de posición de una tarea dentro de la lista de tareas. |
| [IGNORE_RESOURCE_CALENDAR](#IGNORE-RESOURCE-CALENDAR) | Determina si la programación de la tarea considera los calendarios de los recursos asignados a la tarea. |
| [IGNORE_WARNINGS](#IGNORE-WARNINGS) | Indica si se debe ocultar el indicador de advertencia de conflicto de programación en Microsoft Project. |
| [IS_ACTIVE](#IS-ACTIVE) | Determina si una tarea está activa. |
| [IS_CRITICAL](#IS-CRITICAL) | Determina si una tarea está en la ruta crítica. |
| [IS_EFFORT_DRIVEN](#IS-EFFORT-DRIVEN) | Determina si la programación de la tarea es una programación basada en el esfuerzo. |
| [IS_ESTIMATED](#IS-ESTIMATED) | Determina si una tarea es estimada. |
| [IS_EXPANDED](#IS-EXPANDED) | Determina si una tarea de resumen está expandida o no en la vista GanttChart. |
| [IS_EXTERNAL_TASK](#IS-EXTERNAL-TASK) | Determina si una tarea es externa. |
| [IS_MANUAL](#IS-MANUAL) | Determina si una tarea está programada manualmente. |
| [IS_MARKED](#IS-MARKED) | Muestra si una tarea está marcada para una acción adicional o identificación de algún tipo. |
| [IS_MILESTONE](#IS-MILESTONE) | Determina si una tarea es un hito. |
| [IS_NULL](#IS-NULL) | Determina si una tarea es una tarea nula. |
| [IS_OVERALLOCATED](#IS-OVERALLOCATED) | Indica si alguno de los recursos asignados a una tarea está asignado a más trabajo del que se puede realizar dentro de la capacidad de trabajo normal. |
| [IS_PUBLISHED](#IS-PUBLISHED) | Determina si la tarea actual debe publicarse en Project Server junto con el resto del proyecto. |
| [IS_RECURRING](#IS-RECURRING) | Determina si una tarea forma parte de una serie de tareas recurrentes. |
| [IS_RESUME_VALID](#IS-RESUME-VALID) | Determina si una tarea puede reanudarse. |
| [IS_ROLLUP](#IS-ROLLUP) | Determina si la información sobre las barras Gantt de la subtarea se consolidará en la barra de la tarea resumen. |
| [IS_SUBPROJECT](#IS-SUBPROJECT) | Determina si una tarea es un proyecto insertado. |
| [IS_SUBPROJECT_READ_ONLY](#IS-SUBPROJECT-READ-ONLY) | Determina si un subproyecto es de solo lectura. |
| [IS_SUMMARY](#IS-SUMMARY) | Determina si una tarea es una tarea resumen. |
| [LATE_FINISH](#LATE-FINISH) | La fecha más tardía en que una tarea puede finalizar sin retrasar la finalización del proyecto. |
| [LATE_START](#LATE-START) | La fecha más tardía en que una tarea puede iniciar sin retrasar la finalización del proyecto. |
| [LEVELING_CAN_SPLIT](#LEVELING-CAN-SPLIT) | Determina si la función de nivelación de recursos puede causar divisiones en el trabajo restante de esta tarea. |
| [LEVELING_DELAY](#LEVELING-DELAY) | El tiempo que una tarea debe retrasarse desde su fecha de inicio temprana debido a la nivelación de recursos. |
| [LEVEL_ASSIGNMENTS](#LEVEL-ASSIGNMENTS) | Determina si la función de nivelación puede retrasar y dividir asignaciones individuales para resolver sobreasignaciones. |
| [MANUAL_DURATION](#MANUAL-DURATION) | Define la duración programada manualmente de una tarea. |
| [MANUAL_FINISH](#MANUAL-FINISH) | Define la finalización programada manualmente de una tarea. |
| [MANUAL_START](#MANUAL-START) | Define el inicio programado manualmente de una tarea. |
| [NAME](#NAME) | El nombre de una tarea. |
| [NOTES_RTF](#NOTES-RTF) | Las notas de texto en formato RTF. |
| [NOTES_TEXT](#NOTES-TEXT) | Texto plano de las notas extraído de datos RTF. |
| [OUTLINE_LEVEL](#OUTLINE-LEVEL) | El nivel de esquema de una tarea. |
| [OUTLINE_NUMBER](#OUTLINE-NUMBER) | El número que representa la posición de una tarea en la estructura jerárquica del esquema. |
| [OVERTIME_COST](#OVERTIME-COST) | El costo total de horas extra para una tarea, para un recurso en todas las tareas asignadas o para una asignación de recurso. |
| [OVERTIME_WORK](#OVERTIME-WORK) | La cantidad de horas extra programada para ser realizada por todos los recursos asignados a una tarea. |
| [PERCENT_COMPLETE](#PERCENT-COMPLETE) | El estado actual de una tarea, expresado como el porcentaje de la duración de la tarea que se ha completado. |
| [PERCENT_WORK_COMPLETE](#PERCENT-WORK-COMPLETE) | El estado actual de una tarea expresado como el porcentaje del trabajo que se ha completado. |
| [PHYSICAL_PERCENT_COMPLETE](#PHYSICAL-PERCENT-COMPLETE) | Valor de porcentaje completado que puede usarse como alternativa para calcular el costo presupuestado del trabajo realizado (BCWP). |
| [PRELEVELED_FINISH](#PRELEVELED-FINISH) | La fecha de finalización de una tarea tal como estaba antes de que se realizara el nivelado de recursos. |
| [PRELEVELED_START](#PRELEVELED-START) | La fecha de inicio de una tarea tal como estaba antes de que se realizara el nivelado de recursos. |
| [PRIORITY](#PRIORITY) | El nivel de importancia asignado a una tarea, que a su vez indica cuán fácilmente una tarea o asignación puede retrasarse o dividirse durante el nivelado de recursos. |
| [REGULAR_WORK](#REGULAR-WORK) | La cantidad total de trabajo sin horas extra programado para ser realizado por los recursos. |
| [REMAINING_COST](#REMAINING-COST) | El gasto programado restante que se incurrirá al completar el trabajo programado restante. |
| [REMAINING_DURATION](#REMAINING-DURATION) | El tiempo necesario para completar la parte no terminada de una tarea. |
| [REMAINING_OVERTIME_COST](#REMAINING-OVERTIME-COST) | El gasto de horas extra programado restante para una tarea. |
| [REMAINING_OVERTIME_WORK](#REMAINING-OVERTIME-WORK) | La cantidad de tiempo de horas extra programado restante. |
| [REMAINING_WORK](#REMAINING-WORK) | El tiempo aún necesario para completar una tarea o conjunto de tareas. |
| [RESUME](#RESUME) | La fecha en que la parte restante de una tarea está programada para reanudarse después de registrar cualquier progreso. |
| [START](#START) | La fecha de inicio programada de una tarea. |
| [START_SLACK_TIME_SPAN](#START-SLACK-TIME-SPAN) | La duración (en segundos) entre las fechas de Inicio Temprano y Inicio Tardío. |
| [START_TEXT](#START-TEXT) | Devuelve el texto de inicio de la tarea. |
| [START_VARIANCE](#START-VARIANCE) | El tiempo que representa la diferencia entre una fecha de inicio de referencia de una tarea o asignación y su fecha de inicio programada actualmente. |
| [STATUS_MANAGER](#STATUS-MANAGER) | El nombre del recurso empresarial que debe recibir actualizaciones de estado de la tarea actual de los recursos. |
| [STOP](#STOP) | La fecha que representa el final de la parte real de una tarea. |
| [SUBPROJECT_NAME](#SUBPROJECT-NAME) | La ubicación de origen de un subproyecto. |
| [SV](#SV) | La variación del cronograma del valor ganado, hasta la fecha de estado del proyecto. |
| [TOTAL_SLACK_TIME_SPAN](#TOTAL-SLACK-TIME-SPAN) | El tiempo que la fecha de finalización de una tarea puede retrasarse sin retrasar la fecha de finalización del proyecto. |
| [TYPE](#TYPE) | El tipo de una tarea. |
| [UID](#UID) | El Id único de una tarea. |
| [WARNING](#WARNING) | Representa la bandera que indica que la tarea tiene discrepancias de programación. |
| [WBS](#WBS) | Códigos de estructura de desglose del trabajo (WBS). |
| [WBS_LEVEL](#WBS-LEVEL) | El nivel WBS más a la derecha de una tarea. |
| [WORK](#WORK) | El tiempo total programado en una tarea para todos los recursos asignados. |
| [WORK_VARIANCE](#WORK-VARIANCE) | La diferencia entre el trabajo de referencia de una tarea y el trabajo programado actualmente. |
### Tsk() {#Tsk--}
```
public Tsk()
```


### ACTIVITY_ID {#ACTIVITY-ID}
```
public static final Key<String,Byte> ACTIVITY_ID
```


Representa el campo de id de actividad - un identificador único de tarea utilizado por Primavera. (solo aplicable a proyectos Primavera).

### ACTUAL_COST {#ACTUAL-COST}
```
public static final Key<BigDecimal,Byte> ACTUAL_COST
```


Costos incurridos por el trabajo ya realizado por los recursos en sus tareas, junto con cualquier otro costo registrado asociado a la tarea.

### ACTUAL_DURATION {#ACTUAL-DURATION}
```
public static final Key<Duration,Byte> ACTUAL_DURATION
```


El período de tiempo de trabajo real para una tarea, basado en la duración programada y el trabajo restante actual o el porcentaje completado.

### ACTUAL_FINISH {#ACTUAL-FINISH}
```
public static final Key<Date,Byte> ACTUAL_FINISH
```


La fecha en que se completó una tarea.

### ACTUAL_OVERTIME_COST {#ACTUAL-OVERTIME-COST}
```
public static final Key<BigDecimal,Byte> ACTUAL_OVERTIME_COST
```


Costos incurridos por trabajo extra ya realizado en tareas por los recursos asignados.

### ACTUAL_OVERTIME_WORK {#ACTUAL-OVERTIME-WORK}
```
public static final Key<Duration,Byte> ACTUAL_OVERTIME_WORK
```


La cantidad real de trabajo extra ya realizado por los recursos asignados a tareas.

### ACTUAL_OVERTIME_WORK_PROTECTED {#ACTUAL-OVERTIME-WORK-PROTECTED}
```
public static final Key<Duration,Byte> ACTUAL_OVERTIME_WORK_PROTECTED
```


La duración durante la cual el trabajo extra real está protegido.

### ACTUAL_START {#ACTUAL-START}
```
public static final Key<Date,Byte> ACTUAL_START
```


La fecha y hora en que una tarea comenzó realmente.

### ACTUAL_WORK {#ACTUAL-WORK}
```
public static final Key<Duration,Byte> ACTUAL_WORK
```


La cantidad de trabajo que ya se ha realizado por los recursos asignados a las tareas.

### ACTUAL_WORK_PROTECTED {#ACTUAL-WORK-PROTECTED}
```
public static final Key<Duration,Byte> ACTUAL_WORK_PROTECTED
```


La duración durante la cual el trabajo real está protegido.

--------------------

Lectura compatible solo con formato XML.

### ACWP {#ACWP}
```
public static final Key<Double,Byte> ACWP
```


Costos incurridos por el trabajo ya realizado en una tarea, hasta la fecha de estado del proyecto o la fecha de hoy.

### BCWP {#BCWP}
```
public static final Key<Double,Byte> BCWP
```


El valor acumulado del porcentaje de completado de la tarea multiplicado por los costos de referencia basados en tiempo.

### BCWS {#BCWS}
```
public static final Key<Double,Byte> BCWS
```


Los costos de referencia acumulados basados en tiempo hasta la fecha de estado o la fecha de hoy.

### BUDGET_COST {#BUDGET-COST}
```
public static final Key<BigDecimal,Byte> BUDGET_COST
```


Costos presupuestarios para recursos de costo presupuestario. Los recursos presupuestarios se asignan solo a la tarea de resumen del proyecto.

### BUDGET_WORK {#BUDGET-WORK}
```
public static final Key<Duration,Byte> BUDGET_WORK
```


Trabajo presupuestado para trabajo presupuestado y recursos materiales. Los recursos presupuestados se asignan solo a la tarea de resumen del proyecto.

### CALENDAR {#CALENDAR}
```
public static final Key<Calendar,Byte> CALENDAR
```


El calendario de la tarea.

### COMMITMENT_FINISH {#COMMITMENT-FINISH}
```
public static final Key<Date,Byte> COMMITMENT_FINISH
```


La fecha de finalización de una entrega.

--------------------

Lectura compatible solo con formato XML.

### COMMITMENT_START {#COMMITMENT-START}
```
public static final Key<Date,Byte> COMMITMENT_START
```


La fecha de inicio de una entrega.

--------------------

Lectura compatible solo con formato XML.

### COMMITMENT_TYPE {#COMMITMENT-TYPE}
```
public static final Key<Integer,Byte> COMMITMENT_TYPE
```


Determina si una tarea tiene una entrega asociada o una dependencia de una entrega asociada.

--------------------

Lectura compatible solo con formato XML.

### CONSTRAINT_DATE {#CONSTRAINT-DATE}
```
public static final Key<Date,Byte> CONSTRAINT_DATE
```


La fecha específica asociada al tipo de restricción.

### CONSTRAINT_TYPE {#CONSTRAINT-TYPE}
```
public static final Key<Integer,Byte> CONSTRAINT_TYPE
```


Proporciona opciones para el tipo de restricción que se puede aplicar al programar una tarea.

### CONTACT {#CONTACT}
```
public static final Key<String,Byte> CONTACT
```


El nombre de la persona responsable de una tarea.

### COST {#COST}
```
public static final Key<BigDecimal,Byte> COST
```


El costo total programado o proyectado para una tarea basado en los costos ya incurridos por el trabajo realizado por los recursos asignados a las tareas, además de los costos planificados para el trabajo restante.

### COST_VARIANCE {#COST-VARIANCE}
```
public static final Key<Double,Byte> COST_VARIANCE
```


La diferencia entre el costo de referencia y el costo total para una tarea, recurso o asignación.

### CREATED {#CREATED}
```
public static final Key<Date,Byte> CREATED
```


La fecha en que se creó una tarea.

### CV {#CV}
```
public static final Key<Double,Byte> CV
```


La diferencia entre el costo de referencia y el costo total de una tarea. Variación de costo = Costo - Costo de referencia

### DEADLINE {#DEADLINE}
```
public static final Key<Date,Byte> DEADLINE
```


Una fecha objetivo que indica cuándo debe completarse una tarea.

### DISPLAY_AS_SUMMARY {#DISPLAY-AS-SUMMARY}
```
public static final Key<NullableBool,Byte> DISPLAY_AS_SUMMARY
```


Determina si la tarea debe mostrarse como una tarea resumen.

--------------------

Lectura compatible solo con formato XML.

### DISPLAY_ON_TIMELINE {#DISPLAY-ON-TIMELINE}
```
public static final Key<Boolean,Byte> DISPLAY_ON_TIMELINE
```


Especifica si una tarea debe mostrarse en una vista de línea de tiempo.

### DURATION {#DURATION}
```
public static final Key<Duration,Byte> DURATION
```


El período total de tiempo de trabajo activo para una tarea según se ingresó o según lo calcule Microsoft Project basado en la fecha de inicio, fecha de finalización, calendarios y otros factores de programación.

### DURATION_TEXT {#DURATION-TEXT}
```
public static final Key<String,Byte> DURATION_TEXT
```


Devuelve el texto de duración de la tarea.

### DURATION_VARIANCE {#DURATION-VARIANCE}
```
public static final Key<Duration,Byte> DURATION_VARIANCE
```


La diferencia entre la duración de referencia de una tarea y la duración total (estimación actual) de una tarea.

### EARLY_FINISH {#EARLY-FINISH}
```
public static final Key<Date,Byte> EARLY_FINISH
```


La fecha más temprana en que una tarea podría finalizar, basada en las fechas de finalización temprana de las tareas predecesoras y sucesoras, otras restricciones y cualquier retraso de nivelación.

### EARLY_START {#EARLY-START}
```
public static final Key<Date,Byte> EARLY_START
```


La fecha más temprana en que una tarea podría comenzar, basada en las fechas de inicio temprano de las tareas predecesoras y sucesoras y otras restricciones.

### EARNED_VALUE_METHOD {#EARNED-VALUE-METHOD}
```
public static final Key<Integer,Byte> EARNED_VALUE_METHOD
```


Determina si se debe usar el campo % Complete o Physical % Complete para calcular el costo presupuestado del trabajo realizado (BCWP).

### EXTERNAL_ID {#EXTERNAL-ID}
```
public static final Key<Integer,Byte> EXTERNAL_ID
```


Si una tarea es una tarea externa, contiene el Id externo de la tarea.

### EXTERNAL_TASK_PROJECT {#EXTERNAL-TASK-PROJECT}
```
public static final Key<String,Byte> EXTERNAL_TASK_PROJECT
```


La ubicación de origen y el identificador de la tarea de una tarea externa.

### EXTERNAL_UID {#EXTERNAL-UID}
```
public static final Key<Integer,Byte> EXTERNAL_UID
```


Contiene el identificador único de la tarea externa cuando la tarea es externa.

### FINISH {#FINISH}
```
public static final Key<Date,Byte> FINISH
```


La fecha de finalización programada de una tarea.

### FINISH_SLACK_TIME_SPAN {#FINISH-SLACK-TIME-SPAN}
```
public static final Key<TimeDelta,Byte> FINISH_SLACK_TIME_SPAN
```


La duración (en segundos) entre las fechas de Finalización Temprana y Finalización Tardía.

### FINISH_TEXT {#FINISH-TEXT}
```
public static final Key<String,Byte> FINISH_TEXT
```


Devuelve el texto de finalización de la tarea.

### FINISH_VARIANCE {#FINISH-VARIANCE}
```
public static final Key<Duration,Byte> FINISH_VARIANCE
```


El tiempo que representa la diferencia entre la fecha de finalización de referencia de una tarea o asignación y su fecha de finalización actual.

### FIXED_COST {#FIXED-COST}
```
public static final Key<Double,Byte> FIXED_COST
```


Muestra cualquier gasto de tarea que no sea de recurso.

### FIXED_COST_ACCRUAL {#FIXED-COST-ACCRUAL}
```
public static final Key<Integer,Byte> FIXED_COST_ACCRUAL
```


Determina las opciones de cómo y cuándo se deben cargar o acumular los costos fijos al costo de una tarea.

### FREE_SLACK_TIME_SPAN {#FREE-SLACK-TIME-SPAN}
```
public static final Key<TimeDelta,Byte> FREE_SLACK_TIME_SPAN
```


El tiempo (en segundos) que una tarea puede retrasarse sin retrasar ninguna tarea sucesora.

### GUID {#GUID}
```
public static final Key<String,Byte> GUID
```


Los códigos de identificación únicos generados para una tarea.

### HAS_OVERALLOCATED_RESOURCE {#HAS-OVERALLOCATED-RESOURCE}
```
public static final Key<NullableBool,Byte> HAS_OVERALLOCATED_RESOURCE
```


Indica si la tarea tiene un recurso asignado que tiene más trabajo en tareas asignadas del que puede completarse dentro de la capacidad de trabajo normal.

### HIDE_BAR {#HIDE-BAR}
```
public static final Key<NullableBool,Byte> HIDE_BAR
```


Determina si la barra Gantt de una tarea está oculta cuando se muestra en Microsoft Project.

### HYPERLINK {#HYPERLINK}
```
public static final Key<String,Byte> HYPERLINK
```


El título o texto explicativo de un hipervínculo asociado a una tarea.

### HYPERLINK_ADDRESS {#HYPERLINK-ADDRESS}
```
public static final Key<String,Byte> HYPERLINK_ADDRESS
```


La dirección de un hipervínculo asociado a una tarea.

--------------------

La dirección completa (Hyperlink Href en Microsoft Project) del hipervínculo es una concatenación de HyperlinkAddress y HyperlinkSubAddress.

### HYPERLINK_SUB_ADDRESS {#HYPERLINK-SUB-ADDRESS}
```
public static final Key<String,Byte> HYPERLINK_SUB_ADDRESS
```


La ubicación específica en un documento en un hipervínculo asociado a una tarea.

--------------------

La dirección completa (Hyperlink Href en Microsoft Project) del hipervínculo es una concatenación de HyperlinkAddress y HyperlinkSubAddress.

### ID {#ID}
```
public static final Key<Integer,Byte> ID
```


El identificador de posición de una tarea dentro de la lista de tareas.

### IGNORE_RESOURCE_CALENDAR {#IGNORE-RESOURCE-CALENDAR}
```
public static final Key<NullableBool,Byte> IGNORE_RESOURCE_CALENDAR
```


Determina si la programación de la tarea considera los calendarios de los recursos asignados a la tarea.

### IGNORE_WARNINGS {#IGNORE-WARNINGS}
```
public static final Key<Boolean,Byte> IGNORE_WARNINGS
```


Indica si se debe ocultar el indicador de advertencia de conflicto de programación en Microsoft Project.

### IS_ACTIVE {#IS-ACTIVE}
```
public static final Key<NullableBool,Byte> IS_ACTIVE
```


Determina si una tarea está activa. Las tareas inactivas ya no afectan a otras tareas ni al cronograma general del proyecto.

### IS_CRITICAL {#IS-CRITICAL}
```
public static final Key<NullableBool,Byte> IS_CRITICAL
```


Determina si una tarea está en la ruta crítica.

### IS_EFFORT_DRIVEN {#IS-EFFORT-DRIVEN}
```
public static final Key<NullableBool,Byte> IS_EFFORT_DRIVEN
```


Determina si la programación de la tarea es una programación basada en el esfuerzo.

### IS_ESTIMATED {#IS-ESTIMATED}
```
public static final Key<NullableBool,Byte> IS_ESTIMATED
```


Determina si una tarea es estimada.

### IS_EXPANDED {#IS-EXPANDED}
```
public static final Key<NullableBool,Byte> IS_EXPANDED
```


Determina si una tarea de resumen está expandida o no en la vista GanttChart.

### IS_EXTERNAL_TASK {#IS-EXTERNAL-TASK}
```
public static final Key<Boolean,Byte> IS_EXTERNAL_TASK
```


Determina si una tarea es externa.

### IS_MANUAL {#IS-MANUAL}
```
public static final Key<NullableBool,Byte> IS_MANUAL
```


Determina si una tarea está programada manualmente.

### IS_MARKED {#IS-MARKED}
```
public static final Key<Boolean,Byte> IS_MARKED
```


Muestra si una tarea está marcada para una acción adicional o identificación de algún tipo.

--------------------

Se aplica solo al formato de archivo mpp.

### IS_MILESTONE {#IS-MILESTONE}
```
public static final Key<NullableBool,Byte> IS_MILESTONE
```


Determina si una tarea es un hito.

### IS_NULL {#IS-NULL}
```
public static final Key<NullableBool,Byte> IS_NULL
```


Determina si una tarea es una tarea nula.

### IS_OVERALLOCATED {#IS-OVERALLOCATED}
```
public static final Key<NullableBool,Byte> IS_OVERALLOCATED
```


Indica si alguno de los recursos asignados a una tarea está asignado a más trabajo del que se puede realizar dentro de la capacidad de trabajo normal.

### IS_PUBLISHED {#IS-PUBLISHED}
```
public static final Key<NullableBool,Byte> IS_PUBLISHED
```


Determina si la tarea actual debe publicarse en Project Server junto con el resto del proyecto.

### IS_RECURRING {#IS-RECURRING}
```
public static final Key<NullableBool,Byte> IS_RECURRING
```


Determina si una tarea forma parte de una serie de tareas recurrentes.

### IS_RESUME_VALID {#IS-RESUME-VALID}
```
public static final Key<NullableBool,Byte> IS_RESUME_VALID
```


Determina si una tarea puede reanudarse.

### IS_ROLLUP {#IS-ROLLUP}
```
public static final Key<NullableBool,Byte> IS_ROLLUP
```


Determina si la información sobre las barras Gantt de la subtarea se consolidará en la barra de la tarea resumen.

### IS_SUBPROJECT {#IS-SUBPROJECT}
```
public static final Key<Boolean,Byte> IS_SUBPROJECT
```


Determina si una tarea es un proyecto insertado.

### IS_SUBPROJECT_READ_ONLY {#IS-SUBPROJECT-READ-ONLY}
```
public static final Key<NullableBool,Byte> IS_SUBPROJECT_READ_ONLY
```


Determina si un subproyecto es de solo lectura.

### IS_SUMMARY {#IS-SUMMARY}
```
public static final Key<Boolean,Byte> IS_SUMMARY
```


Determina si una tarea es una tarea resumen.

### LATE_FINISH {#LATE-FINISH}
```
public static final Key<Date,Byte> LATE_FINISH
```


La fecha más tardía en que una tarea puede finalizar sin retrasar la finalización del proyecto.

### LATE_START {#LATE-START}
```
public static final Key<Date,Byte> LATE_START
```


La fecha más tardía en que una tarea puede iniciar sin retrasar la finalización del proyecto.

### LEVELING_CAN_SPLIT {#LEVELING-CAN-SPLIT}
```
public static final Key<NullableBool,Byte> LEVELING_CAN_SPLIT
```


Determina si la función de nivelación de recursos puede causar divisiones en el trabajo restante de esta tarea.

### LEVELING_DELAY {#LEVELING-DELAY}
```
public static final Key<Duration,Byte> LEVELING_DELAY
```


El tiempo que una tarea debe retrasarse desde su fecha de inicio temprana debido a la nivelación de recursos.

### LEVEL_ASSIGNMENTS {#LEVEL-ASSIGNMENTS}
```
public static final Key<NullableBool,Byte> LEVEL_ASSIGNMENTS
```


Determina si la función de nivelación puede retrasar y dividir asignaciones individuales para resolver sobreasignaciones.

### MANUAL_DURATION {#MANUAL-DURATION}
```
public static final Key<Duration,Byte> MANUAL_DURATION
```


Define la duración programada manualmente de una tarea.

### MANUAL_FINISH {#MANUAL-FINISH}
```
public static final Key<Date,Byte> MANUAL_FINISH
```


Define la finalización programada manualmente de una tarea.

### MANUAL_START {#MANUAL-START}
```
public static final Key<Date,Byte> MANUAL_START
```


Define el inicio programado manualmente de una tarea.

### NAME {#NAME}
```
public static final Key<String,Byte> NAME
```


El nombre de una tarea.

### NOTES_RTF {#NOTES-RTF}
```
public static final Key<String,Byte> NOTES_RTF
```


Las notas de texto en formato RTF.

--------------------

Compatible solo con formatos MPP.

### NOTES_TEXT {#NOTES-TEXT}
```
public static final Key<String,Byte> NOTES_TEXT
```


Texto plano de las notas extraído de datos RTF.

### OUTLINE_LEVEL {#OUTLINE-LEVEL}
```
public static final Key<Integer,Byte> OUTLINE_LEVEL
```


El nivel de esquema de una tarea.

### OUTLINE_NUMBER {#OUTLINE-NUMBER}
```
public static final Key<String,Byte> OUTLINE_NUMBER
```


El número que representa la posición de una tarea en la estructura jerárquica del esquema.

### OVERTIME_COST {#OVERTIME-COST}
```
public static final Key<BigDecimal,Byte> OVERTIME_COST
```


El costo total de horas extra para una tarea, para un recurso en todas las tareas asignadas o para una asignación de recurso.

### OVERTIME_WORK {#OVERTIME-WORK}
```
public static final Key<Duration,Byte> OVERTIME_WORK
```


La cantidad de horas extra programada para ser realizada por todos los recursos asignados a una tarea.

### PERCENT_COMPLETE {#PERCENT-COMPLETE}
```
public static final Key<Integer,Byte> PERCENT_COMPLETE
```


El estado actual de una tarea, expresado como el porcentaje de la duración de la tarea que se ha completado.

### PERCENT_WORK_COMPLETE {#PERCENT-WORK-COMPLETE}
```
public static final Key<Integer,Byte> PERCENT_WORK_COMPLETE
```


El estado actual de una tarea expresado como el porcentaje del trabajo que se ha completado.

### PHYSICAL_PERCENT_COMPLETE {#PHYSICAL-PERCENT-COMPLETE}
```
public static final Key<Integer,Byte> PHYSICAL_PERCENT_COMPLETE
```


Valor de porcentaje completado que puede usarse como alternativa para calcular el costo presupuestado del trabajo realizado (BCWP).

### PRELEVELED_FINISH {#PRELEVELED-FINISH}
```
public static final Key<Date,Byte> PRELEVELED_FINISH
```


La fecha de finalización de una tarea tal como estaba antes de que se realizara el nivelado de recursos.

### PRELEVELED_START {#PRELEVELED-START}
```
public static final Key<Date,Byte> PRELEVELED_START
```


La fecha de inicio de una tarea tal como estaba antes de que se realizara el nivelado de recursos.

### PRIORITY {#PRIORITY}
```
public static final Key<Integer,Byte> PRIORITY
```


El nivel de importancia asignado a una tarea, que a su vez indica cuán fácilmente una tarea o asignación puede retrasarse o dividirse durante el nivelado de recursos.

### REGULAR_WORK {#REGULAR-WORK}
```
public static final Key<Duration,Byte> REGULAR_WORK
```


La cantidad total de trabajo sin horas extra programado para ser realizado por los recursos.

### REMAINING_COST {#REMAINING-COST}
```
public static final Key<BigDecimal,Byte> REMAINING_COST
```


El gasto programado restante que se incurrirá al completar el trabajo programado restante.

### REMAINING_DURATION {#REMAINING-DURATION}
```
public static final Key<Duration,Byte> REMAINING_DURATION
```


El tiempo necesario para completar la parte no terminada de una tarea.

### REMAINING_OVERTIME_COST {#REMAINING-OVERTIME-COST}
```
public static final Key<BigDecimal,Byte> REMAINING_OVERTIME_COST
```


El gasto de horas extra programado restante para una tarea.

### REMAINING_OVERTIME_WORK {#REMAINING-OVERTIME-WORK}
```
public static final Key<Duration,Byte> REMAINING_OVERTIME_WORK
```


La cantidad de tiempo de horas extra programado restante.

### REMAINING_WORK {#REMAINING-WORK}
```
public static final Key<Duration,Byte> REMAINING_WORK
```


El tiempo aún necesario para completar una tarea o conjunto de tareas.

### RESUME {#RESUME}
```
public static final Key<Date,Byte> RESUME
```


La fecha en que la parte restante de una tarea está programada para reanudarse después de registrar cualquier progreso.

### START {#START}
```
public static final Key<Date,Byte> START
```


La fecha de inicio programada de una tarea.

### START_SLACK_TIME_SPAN {#START-SLACK-TIME-SPAN}
```
public static final Key<TimeDelta,Byte> START_SLACK_TIME_SPAN
```


La duración (en segundos) entre las fechas de Inicio Temprano y Inicio Tardío.

### START_TEXT {#START-TEXT}
```
public static final Key<String,Byte> START_TEXT
```


Devuelve el texto de inicio de la tarea.

### START_VARIANCE {#START-VARIANCE}
```
public static final Key<Duration,Byte> START_VARIANCE
```


El tiempo que representa la diferencia entre una fecha de inicio de referencia de una tarea o asignación y su fecha de inicio programada actualmente.

### STATUS_MANAGER {#STATUS-MANAGER}
```
public static final Key<String,Byte> STATUS_MANAGER
```


El nombre del recurso empresarial que debe recibir actualizaciones de estado de la tarea actual de los recursos.

### STOP {#STOP}
```
public static final Key<Date,Byte> STOP
```


La fecha que representa el final de la parte real de una tarea.

### SUBPROJECT_NAME {#SUBPROJECT-NAME}
```
public static final Key<String,Byte> SUBPROJECT_NAME
```


La ubicación de origen de un subproyecto.

### SV {#SV}
```
public static final Key<Double,Byte> SV
```


La variación del cronograma del valor ganado, hasta la fecha de estado del proyecto. La variación del cronograma (SV) es la diferencia entre el BCWP y el BCWS.

### TOTAL_SLACK_TIME_SPAN {#TOTAL-SLACK-TIME-SPAN}
```
public static final Key<TimeDelta,Byte> TOTAL_SLACK_TIME_SPAN
```


El tiempo que la fecha de finalización de una tarea puede retrasarse sin retrasar la fecha de finalización del proyecto.

### TYPE {#TYPE}
```
public static final Key<Integer,Byte> TYPE
```


El tipo de una tarea.

### UID {#UID}
```
public static final Key<Integer,Byte> UID
```


El Id único de una tarea.

### WARNING {#WARNING}
```
public static final Key<Boolean,Byte> WARNING
```


Representa la bandera que indica que la tarea tiene discrepancias de programación.

### WBS {#WBS}
```
public static final Key<String,Byte> WBS
```


Códigos de estructura de desglose del trabajo (WBS).

### WBS_LEVEL {#WBS-LEVEL}
```
public static final Key<String,Byte> WBS_LEVEL
```


El nivel WBS más a la derecha de una tarea.

### WORK {#WORK}
```
public static final Key<Duration,Byte> WORK
```


El tiempo total programado en una tarea para todos los recursos asignados.

### WORK_VARIANCE {#WORK-VARIANCE}
```
public static final Key<Duration,Byte> WORK_VARIANCE
```


La diferencia entre el trabajo de referencia de una tarea y el trabajo programado actualmente.

