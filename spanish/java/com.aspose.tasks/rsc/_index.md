---
title: "Rsc"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Representa las propiedades compatibles del objeto Resource."
type: docs
weight: 271
url: /es/java/com.aspose.tasks/rsc/
---

**Inheritance:**
java.lang.Object
```
public class Rsc
```

Representa las propiedades compatibles del objeto `Resource`.
## Campos

| Campo | Descripción |
| --- | --- |
| [ACCRUE_AT](#ACCRUE-AT) | Determina cómo y cuándo se deben cargar, o acumular, los costos estándar y de horas extra del recurso al costo de una tarea. |
| [ACTIVE_DIRECTORY_GUID](#ACTIVE-DIRECTORY-GUID) | El GUID de Active Directory para un recurso. |
| [ACTUAL_COST](#ACTUAL-COST) | Costos incurridos por el trabajo ya realizado por los recursos en sus tareas, junto con cualquier otro costo registrado asociado a la tarea. |
| [ACTUAL_OVERTIME_COST](#ACTUAL-OVERTIME-COST) | Costos incurridos por trabajo extra ya realizado en tareas por los recursos asignados. |
| [ACTUAL_OVERTIME_WORK](#ACTUAL-OVERTIME-WORK) | La cantidad real de trabajo extra ya realizado por el recurso asignado a tareas. |
| [ACTUAL_OVERTIME_WORK_PROTECTED](#ACTUAL-OVERTIME-WORK-PROTECTED) | La cantidad de trabajo a través de la cual el trabajo extra real está protegido. |
| [ACTUAL_WORK](#ACTUAL-WORK) | La cantidad de trabajo que ya ha sido realizado por el recurso asignado a tareas. |
| [ACTUAL_WORK_PROTECTED](#ACTUAL-WORK-PROTECTED) | La cantidad de trabajo a través de la cual el trabajo real está protegido. |
| [ACWP](#ACWP) | El costo real de un trabajo realizado por un recurso para el proyecto hasta la fecha. |
| [ASSIGNMENT_OWNER](#ASSIGNMENT-OWNER) | El nombre del propietario de la asignación. |
| [ASSIGNMENT_OWNER_GUID](#ASSIGNMENT-OWNER-GUID) | El GUID del propietario de la asignación. |
| [AVAILABLE_FROM](#AVAILABLE-FROM) | La fecha de inicio en que un recurso está disponible para trabajar en las unidades especificadas para el período de tiempo actual. |
| [AVAILABLE_TO](#AVAILABLE-TO) | La fecha de finalización en que un recurso está disponible para trabajar en las unidades especificadas para el período de tiempo actual. |
| [BCWP](#BCWP) | El costo presupuestado de un trabajo realizado por un recurso para el proyecto hasta la fecha. |
| [BCWS](#BCWS) | El costo presupuestario de un trabajo programado para un recurso. |
| [BOOKING_TYPE](#BOOKING-TYPE) | El tipo de reserva de un recurso. |
| [BUDGET_COST](#BUDGET-COST) | Costos presupuestarios para recursos de costo presupuestario. |
| [BUDGET_WORK](#BUDGET-WORK) | Trabajo presupuestado para trabajo presupuestado y recursos materiales. |
| [CALENDAR](#CALENDAR) | El calendario de un recurso. |
| [CAN_LEVEL](#CAN-LEVEL) | Determina si se puede realizar nivelación de recursos en un recurso. |
| [CODE](#CODE) | El código u otra información sobre un recurso. |
| [COST](#COST) | El costo total programado o proyectado para un recurso, basado en los costos ya incurridos por el trabajo realizado por los recursos asignados a las tareas, además de los costos planificados para el trabajo restante. |
| [COST_CENTER](#COST-CENTER) | Indica a qué centro de costos se deben cargar los costos acumulados por el recurso. |
| [COST_PER_USE](#COST-PER-USE) | El costo que se acumula cada vez que se utiliza un recurso. |
| [COST_VARIANCE](#COST-VARIANCE) | La diferencia entre el costo base y el costo total para un recurso. |
| [CREATED](#CREATED) | La fecha y hora en que un recurso fue añadido al proyecto. |
| [CV](#CV) | La variación del costo del valor ganado, hasta la fecha de estado del proyecto. |
| [E_MAIL_ADDRESS](#E-MAIL-ADDRESS) | La dirección de correo electrónico de un recurso. |
| [FINISH](#FINISH) | La fecha en que se programa que un recurso complete el trabajo en todas las tareas asignadas. |
| [GROUP](#GROUP) | El grupo al que pertenece un recurso. |
| [GUID](#GUID) | Contiene el código de identificación único generado para el recurso. |
| [HYPERLINK](#HYPERLINK) | El título o texto explicativo de un hipervínculo asociado a un recurso. |
| [HYPERLINK_ADDRESS](#HYPERLINK-ADDRESS) | La dirección de un hipervínculo asociado a un recurso. |
| [HYPERLINK_SUB_ADDRESS](#HYPERLINK-SUB-ADDRESS) | La ubicación específica en un documento en un hipervínculo asociado a una tarea. |
| [ID](#ID) | El identificador de posición de un recurso dentro de la lista de recursos. |
| [INACTIVE](#INACTIVE) | Determina si un recurso fue inactivado por un usuario que tiene derechos administrativos. |
| [INITIALS](#INITIALS) | Las iniciales de un recurso. |
| [IS_BUDGET](#IS-BUDGET) | Determina si un recurso de trabajo, material o costo es un recurso presupuestario. |
| [IS_COST_RESOURCE](#IS-COST-RESOURCE) | Determina si un recurso es un recurso de costo. |
| [IS_ENTERPRISE](#IS-ENTERPRISE) | Muestra si un recurso proviene del grupo de recursos empresarial (true) o del grupo de recursos local (false). |
| [IS_GENERIC](#IS-GENERIC) | Determina si un recurso es genérico o no. |
| [IS_NULL](#IS-NULL) | Determina si un recurso es nulo. |
| [IS_TEAM_ASSIGNMENT_POOL](#IS-TEAM-ASSIGNMENT-POOL) | Muestra si el recurso actual es un recurso de equipo. |
| [MATERIAL_LABEL](#MATERIAL-LABEL) | La unidad de medida del recurso material. |
| [MAX_UNITS](#MAX-UNITS) | El número máximo de unidades que representa la capacidad máxima para la cual un recurso está disponible para realizar cualquier tarea durante el período de tiempo actual. |
| [NAME](#NAME) | El nombre de un recurso. |
| [NOTES_RTF](#NOTES-RTF) | Las notas de texto en formato RTF. |
| [NOTES_TEXT](#NOTES-TEXT) | Texto plano de las notas extraído de datos RTF. |
| [OVERALLOCATED](#OVERALLOCATED) | Indica si un recurso está asignado a más trabajo en una tarea específica o en todas las tareas de lo que se puede completar dentro de la capacidad de trabajo normal. |
| [OVERTIME_COST](#OVERTIME-COST) | El costo total de horas extra para un recurso en todas las tareas asignadas. |
| [OVERTIME_RATE](#OVERTIME-RATE) | La tarifa de pago por el trabajo extra realizado por un recurso. |
| [OVERTIME_RATE_FORMAT](#OVERTIME-RATE-FORMAT) | Las unidades utilizadas por Microsoft Project para mostrar la tarifa de horas extra. |
| [OVERTIME_WORK](#OVERTIME-WORK) | La cantidad de horas extra programada para ser realizada por un recurso en una tarea y cobrada según las tarifas de horas extra de los recursos involucrados. |
| [PEAK_UNITS](#PEAK-UNITS) | La unidad máxima de asignación para un recurso en cualquier momento para todas las tareas a las que el recurso está asignado. |
| [PERCENT_WORK_COMPLETE](#PERCENT-WORK-COMPLETE) | El porcentaje de trabajo completado en todas las tareas. |
| [PHONETICS](#PHONETICS) | La ortografía fonética del nombre del recurso. |
| [REGULAR_WORK](#REGULAR-WORK) | La cantidad total de trabajo sin horas extra programado para ser realizado por el recurso. |
| [REMAINING_COST](#REMAINING-COST) | El gasto programado restante que se incurrirá al completar el trabajo programado restante. |
| [REMAINING_OVERTIME_COST](#REMAINING-OVERTIME-COST) | El gasto de horas extra programado restante para un recurso. |
| [REMAINING_OVERTIME_WORK](#REMAINING-OVERTIME-WORK) | La cantidad de horas extra programada restante. |
| [REMAINING_WORK](#REMAINING-WORK) | El tiempo aún necesario para completar una tarea o conjunto de tareas. |
| [STANDARD_RATE](#STANDARD-RATE) | La tarifa de pago para el trabajo regular, sin horas extra, realizado por un recurso. |
| [STANDARD_RATE_FORMAT](#STANDARD-RATE-FORMAT) | Las unidades utilizadas por Microsoft Project para mostrar la tarifa estándar. |
| [START](#START) | La fecha en que un recurso asignado está programado para comenzar a trabajar en una tarea. |
| [SV](#SV) | La variación del cronograma del valor ganado, hasta la fecha de estado del proyecto. |
| [TYPE](#TYPE) | El tipo de un recurso. |
| [UID](#UID) | El identificador único de un recurso. |
| [WINDOWS_USER_ACCOUNT](#WINDOWS-USER-ACCOUNT) | La cuenta NT asociada a un recurso. |
| [WORK](#WORK) | La cantidad total de tiempo programado para un recurso en una tarea. |
| [WORKGROUP](#WORKGROUP) | El tipo de grupo de trabajo al que pertenece un recurso. |
| [WORK_VARIANCE](#WORK-VARIANCE) | La diferencia entre el trabajo de referencia de un recurso y el trabajo programado actualmente. |
### ACCRUE_AT {#ACCRUE-AT}
```
public static final Key<Integer,Byte> ACCRUE_AT
```


Determina cómo y cuándo se deben cargar, o acumular, los costos estándar y de horas extra del recurso al costo de una tarea.

### ACTIVE_DIRECTORY_GUID {#ACTIVE-DIRECTORY-GUID}
```
public static final Key<String,Byte> ACTIVE_DIRECTORY_GUID
```


El GUID de Active Directory para un recurso.

### ACTUAL_COST {#ACTUAL-COST}
```
public static final Key<BigDecimal,Byte> ACTUAL_COST
```


Costos incurridos por el trabajo ya realizado por los recursos en sus tareas, junto con cualquier otro costo registrado asociado a la tarea.

### ACTUAL_OVERTIME_COST {#ACTUAL-OVERTIME-COST}
```
public static final Key<BigDecimal,Byte> ACTUAL_OVERTIME_COST
```


Costos incurridos por trabajo extra ya realizado en tareas por los recursos asignados.

### ACTUAL_OVERTIME_WORK {#ACTUAL-OVERTIME-WORK}
```
public static final Key<Duration,Byte> ACTUAL_OVERTIME_WORK
```


La cantidad real de trabajo extra ya realizado por el recurso asignado a tareas.

### ACTUAL_OVERTIME_WORK_PROTECTED {#ACTUAL-OVERTIME-WORK-PROTECTED}
```
public static final Key<Duration,Byte> ACTUAL_OVERTIME_WORK_PROTECTED
```


La cantidad de trabajo a través de la cual el trabajo extra real está protegido.

### ACTUAL_WORK {#ACTUAL-WORK}
```
public static final Key<Duration,Byte> ACTUAL_WORK
```


La cantidad de trabajo que ya ha sido realizado por el recurso asignado a tareas.

### ACTUAL_WORK_PROTECTED {#ACTUAL-WORK-PROTECTED}
```
public static final Key<Duration,Byte> ACTUAL_WORK_PROTECTED
```


La cantidad de trabajo a través de la cual el trabajo real está protegido.

### ACWP {#ACWP}
```
public static final Key<Double,Byte> ACWP
```


El costo real de un trabajo realizado por un recurso para el proyecto hasta la fecha.

### ASSIGNMENT_OWNER {#ASSIGNMENT-OWNER}
```
public static final Key<String,Byte> ASSIGNMENT_OWNER
```


El nombre del propietario de la asignación.

### ASSIGNMENT_OWNER_GUID {#ASSIGNMENT-OWNER-GUID}
```
public static final Key<String,Byte> ASSIGNMENT_OWNER_GUID
```


El GUID del propietario de la asignación.

### AVAILABLE_FROM {#AVAILABLE-FROM}
```
public static final Key<Date,Byte> AVAILABLE_FROM
```


La fecha de inicio en que un recurso está disponible para trabajar en las unidades especificadas para el período de tiempo actual.

### AVAILABLE_TO {#AVAILABLE-TO}
```
public static final Key<Date,Byte> AVAILABLE_TO
```


La fecha de finalización en que un recurso está disponible para trabajar en las unidades especificadas para el período de tiempo actual.

### BCWP {#BCWP}
```
public static final Key<Double,Byte> BCWP
```


El costo presupuestado de un trabajo realizado por un recurso para el proyecto hasta la fecha.

### BCWS {#BCWS}
```
public static final Key<Double,Byte> BCWS
```


El costo presupuestario de un trabajo programado para un recurso.

### BOOKING_TYPE {#BOOKING-TYPE}
```
public static final Key<Integer,Byte> BOOKING_TYPE
```


El tipo de reserva de un recurso.

### BUDGET_COST {#BUDGET-COST}
```
public static final Key<BigDecimal,Byte> BUDGET_COST
```


Costos presupuestarios para recursos de costo presupuestario. Los recursos presupuestarios se asignan solo a la tarea de resumen del proyecto.

### BUDGET_WORK {#BUDGET-WORK}
```
public static final Key<Duration,Byte> BUDGET_WORK
```


Trabajo presupuestado para recursos de trabajo presupuestado y materiales. Los recursos presupuestarios se asignan solo a la tarea de resumen del proyecto.

### CALENDAR {#CALENDAR}
```
public static final Key<Calendar,Byte> CALENDAR
```


El calendario de un recurso.

### CAN_LEVEL {#CAN-LEVEL}
```
public static final Key<NullableBool,Byte> CAN_LEVEL
```


Determina si se puede realizar nivelación de recursos en un recurso.

### CODE {#CODE}
```
public static final Key<String,Byte> CODE
```


El código u otra información sobre un recurso.

### COST {#COST}
```
public static final Key<BigDecimal,Byte> COST
```


El costo total programado o proyectado para un recurso, basado en los costos ya incurridos por el trabajo realizado por los recursos asignados a las tareas, además de los costos planificados para el trabajo restante.

### COST_CENTER {#COST-CENTER}
```
public static final Key<String,Byte> COST_CENTER
```


Indica a qué centro de costos se deben cargar los costos acumulados por el recurso.

### COST_PER_USE {#COST-PER-USE}
```
public static final Key<BigDecimal,Byte> COST_PER_USE
```


El costo que se acumula cada vez que se utiliza un recurso.

### COST_VARIANCE {#COST-VARIANCE}
```
public static final Key<Double,Byte> COST_VARIANCE
```


La diferencia entre el costo base y el costo total para un recurso.

### CREATED {#CREATED}
```
public static final Key<Date,Byte> CREATED
```


La fecha y hora en que un recurso fue añadido al proyecto.

### CV {#CV}
```
public static final Key<Double,Byte> CV
```


La variación del costo del valor ganado, hasta la fecha de estado del proyecto. CV es la diferencia entre el BCWP (costo presupuestado del trabajo realizado) y el ACWP (costo real del trabajo realizado) de la tarea.

### E_MAIL_ADDRESS {#E-MAIL-ADDRESS}
```
public static final Key<String,Byte> E_MAIL_ADDRESS
```


La dirección de correo electrónico de un recurso.

### FINISH {#FINISH}
```
public static final Key<Date,Byte> FINISH
```


La fecha en que se programa que un recurso complete el trabajo en todas las tareas asignadas.

### GROUP {#GROUP}
```
public static final Key<String,Byte> GROUP
```


El grupo al que pertenece un recurso.

### GUID {#GUID}
```
public static final Key<String,Byte> GUID
```


Contiene el código de identificación único generado para el recurso.

### HYPERLINK {#HYPERLINK}
```
public static final Key<String,Byte> HYPERLINK
```


El título o texto explicativo de un hipervínculo asociado a un recurso.

### HYPERLINK_ADDRESS {#HYPERLINK-ADDRESS}
```
public static final Key<String,Byte> HYPERLINK_ADDRESS
```


La dirección de un hipervínculo asociado a un recurso.

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


El identificador de posición de un recurso dentro de la lista de recursos.

### INACTIVE {#INACTIVE}
```
public static final Key<NullableBool,Byte> INACTIVE
```


Determina si un recurso fue inactivado por un usuario que tiene derechos administrativos.

### INITIALS {#INITIALS}
```
public static final Key<String,Byte> INITIALS
```


Las iniciales de un recurso.

### IS_BUDGET {#IS-BUDGET}
```
public static final Key<NullableBool,Byte> IS_BUDGET
```


Determina si un recurso de trabajo, material o costo es un recurso presupuestario.

### IS_COST_RESOURCE {#IS-COST-RESOURCE}
```
public static final Key<NullableBool,Byte> IS_COST_RESOURCE
```


Determina si un recurso es un recurso de costo.

### IS_ENTERPRISE {#IS-ENTERPRISE}
```
public static final Key<NullableBool,Byte> IS_ENTERPRISE
```


Muestra si un recurso proviene del grupo de recursos empresarial (true) o del grupo de recursos local (false).

### IS_GENERIC {#IS-GENERIC}
```
public static final Key<NullableBool,Byte> IS_GENERIC
```


Determina si un recurso es genérico o no.

### IS_NULL {#IS-NULL}
```
public static final Key<NullableBool,Byte> IS_NULL
```


Determina si un recurso es nulo.

### IS_TEAM_ASSIGNMENT_POOL {#IS-TEAM-ASSIGNMENT-POOL}
```
public static final Key<Boolean,Byte> IS_TEAM_ASSIGNMENT_POOL
```


Muestra si el recurso actual es un recurso de equipo.

### MATERIAL_LABEL {#MATERIAL-LABEL}
```
public static final Key<String,Byte> MATERIAL_LABEL
```


La unidad de medida del recurso material.

### MAX_UNITS {#MAX-UNITS}
```
public static final Key<Double,Byte> MAX_UNITS
```


El número máximo de unidades que representa la capacidad máxima para la cual un recurso está disponible para realizar cualquier tarea durante el período de tiempo actual.

### NAME {#NAME}
```
public static final Key<String,Byte> NAME
```


El nombre de un recurso.

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

### OVERALLOCATED {#OVERALLOCATED}
```
public static final Key<NullableBool,Byte> OVERALLOCATED
```


Indica si un recurso está asignado a más trabajo en una tarea específica o en todas las tareas de lo que se puede completar dentro de la capacidad de trabajo normal.

### OVERTIME_COST {#OVERTIME-COST}
```
public static final Key<BigDecimal,Byte> OVERTIME_COST
```


El costo total de horas extra para un recurso en todas las tareas asignadas.

### OVERTIME_RATE {#OVERTIME-RATE}
```
public static final Key<BigDecimal,Byte> OVERTIME_RATE
```


La tarifa de pago por el trabajo extra realizado por un recurso.

### OVERTIME_RATE_FORMAT {#OVERTIME-RATE-FORMAT}
```
public static final Key<Integer,Byte> OVERTIME_RATE_FORMAT
```


Las unidades utilizadas por Microsoft Project para mostrar la tarifa de horas extra.

### OVERTIME_WORK {#OVERTIME-WORK}
```
public static final Key<Duration,Byte> OVERTIME_WORK
```


La cantidad de horas extra programada para ser realizada por un recurso en una tarea y cobrada según las tarifas de horas extra de los recursos involucrados.

### PEAK_UNITS {#PEAK-UNITS}
```
public static final Key<Double,Byte> PEAK_UNITS
```


La unidad máxima de asignación para un recurso en cualquier momento para todas las tareas a las que el recurso está asignado.

### PERCENT_WORK_COMPLETE {#PERCENT-WORK-COMPLETE}
```
public static final Key<Integer,Byte> PERCENT_WORK_COMPLETE
```


El porcentaje de trabajo completado en todas las tareas.

### PHONETICS {#PHONETICS}
```
public static final Key<String,Byte> PHONETICS
```


La ortografía fonética del nombre del recurso. Solo para uso con japonés.

### REGULAR_WORK {#REGULAR-WORK}
```
public static final Key<Duration,Byte> REGULAR_WORK
```


La cantidad total de trabajo sin horas extra programado para ser realizado por el recurso.

### REMAINING_COST {#REMAINING-COST}
```
public static final Key<BigDecimal,Byte> REMAINING_COST
```


El gasto programado restante que se incurrirá al completar el trabajo programado restante.

### REMAINING_OVERTIME_COST {#REMAINING-OVERTIME-COST}
```
public static final Key<BigDecimal,Byte> REMAINING_OVERTIME_COST
```


El gasto de horas extra programado restante para un recurso.

### REMAINING_OVERTIME_WORK {#REMAINING-OVERTIME-WORK}
```
public static final Key<Duration,Byte> REMAINING_OVERTIME_WORK
```


La cantidad de horas extra programada restante.

### REMAINING_WORK {#REMAINING-WORK}
```
public static final Key<Duration,Byte> REMAINING_WORK
```


El tiempo aún necesario para completar una tarea o conjunto de tareas.

### STANDARD_RATE {#STANDARD-RATE}
```
public static final Key<BigDecimal,Byte> STANDARD_RATE
```


La tarifa de pago para el trabajo regular, sin horas extra, realizado por un recurso.

### STANDARD_RATE_FORMAT {#STANDARD-RATE-FORMAT}
```
public static final Key<Integer,Byte> STANDARD_RATE_FORMAT
```


Las unidades utilizadas por Microsoft Project para mostrar la tarifa estándar.

### START {#START}
```
public static final Key<Date,Byte> START
```


La fecha en que un recurso asignado está programado para comenzar a trabajar en una tarea.

### SV {#SV}
```
public static final Key<Double,Byte> SV
```


La variación del cronograma del valor ganado, hasta la fecha de estado del proyecto. SV es la diferencia entre el costo presupuestado del trabajo realizado (BCWP) y el costo presupuestado del trabajo programado (BCWS).

### TYPE {#TYPE}
```
public static final Key<Integer,Byte> TYPE
```


El tipo de un recurso.

### UID {#UID}
```
public static final Key<Integer,Byte> UID
```


El identificador único de un recurso.

### WINDOWS_USER_ACCOUNT {#WINDOWS-USER-ACCOUNT}
```
public static final Key<String,Byte> WINDOWS_USER_ACCOUNT
```


La cuenta NT asociada a un recurso.

### WORK {#WORK}
```
public static final Key<Duration,Byte> WORK
```


La cantidad total de tiempo programado para un recurso en una tarea.

### WORKGROUP {#WORKGROUP}
```
public static final Key<Integer,Byte> WORKGROUP
```


El tipo de grupo de trabajo al que pertenece un recurso.

### WORK_VARIANCE {#WORK-VARIANCE}
```
public static final Key<Double,Byte> WORK_VARIANCE
```


La diferencia entre el trabajo de referencia de un recurso y el trabajo programado actualmente.

