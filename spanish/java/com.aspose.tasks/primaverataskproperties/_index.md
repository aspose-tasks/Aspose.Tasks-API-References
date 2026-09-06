---
title: "PrimaveraTaskProperties"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Representa propiedades específicas de Primavera para una tarea leída de los archivos Primavera XER o P6XML."
type: docs
weight: 209
url: /es/java/com.aspose.tasks/primaverataskproperties/
---

**Inheritance:**
java.lang.Object
```
public final class PrimaveraTaskProperties
```

Representa propiedades específicas de Primavera para una tarea leída de archivos Primavera (XER o P6XML).
## Métodos

| Método | Descripción |
| --- | --- |
| [getActivityId()](#getActivityId--) | Obtiene un campo de id de actividad - el identificador único de la tarea utilizado por Primavera. |
| [getActivityType()](#getActivityType--) | Obtiene el valor del campo 'Activity Type'. |
| [getActualExpenseCost()](#getActualExpenseCost--) | Obtiene el valor del costo real del gasto. |
| [getActualLaborCost()](#getActualLaborCost--) | Obtiene el valor del costo laboral real. |
| [getActualLaborUnits()](#getActualLaborUnits--) | Obtiene el valor de las unidades laborales reales. |
| [getActualMaterialCost()](#getActualMaterialCost--) | Obtiene el valor del costo material real. |
| [getActualNonLaborUnits()](#getActualNonLaborUnits--) | Obtiene el valor de las unidades no laborales reales. |
| [getActualNonlaborCost()](#getActualNonlaborCost--) | Obtiene el valor del costo no laboral real. |
| [getActualTotalCost()](#getActualTotalCost--) | Obtiene el valor total de los costos reales. |
| [getBudgetedExpenseCost()](#getBudgetedExpenseCost--) | Obtiene el valor del costo presupuestado (o planificado) de gastos. |
| [getBudgetedLaborCost()](#getBudgetedLaborCost--) | Obtiene el valor del costo laboral presupuestado (o planificado). |
| [getBudgetedMaterialCost()](#getBudgetedMaterialCost--) | Obtiene el valor del costo material presupuestado (o planificado). |
| [getBudgetedNonlaborCost()](#getBudgetedNonlaborCost--) | Obtiene el valor del costo no laboral presupuestado (o planificado). |
| [getBudgetedTotalCost()](#getBudgetedTotalCost--) | Obtiene el valor total de los costos presupuestados (o planificados). |
| [getDurationPercentComplete()](#getDurationPercentComplete--) | Obtiene el valor del porcentaje completado de la duración. |
| [getDurationType()](#getDurationType--) | Obtiene el valor del campo 'Duration Type' de la actividad. |
| [getPercentCompleteType()](#getPercentCompleteType--) | Obtiene el valor del campo '% Complete Type' de la actividad. |
| [getPhysicalPercentComplete()](#getPhysicalPercentComplete--) | Obtiene el valor de Physical Percent Complete. |
| [getPlannedDuration()](#getPlannedDuration--) | Obtiene la duración original o planificada -- el tiempo total de trabajo desde la fecha de inicio planificada de la tarea hasta la fecha de finalización planificada. |
| [getPrimaryConstraintDate()](#getPrimaryConstraintDate--) | Obtiene la fecha de la restricción primaria. |
| [getPrimaryConstraintType()](#getPrimaryConstraintType--) | Obtiene un tipo de restricción primaria. |
| [getRawActivityType()](#getRawActivityType--) | Obtiene la representación de texto sin formato (como en el archivo fuente) del campo 'Activity Type' de la actividad. |
| [getRawCompletePercentType()](#getRawCompletePercentType--) | Obtiene la representación de texto sin formato (como en el archivo fuente) del campo '% Complete Type' de la actividad. |
| [getRawDurationType()](#getRawDurationType--) | Obtiene la representación de texto sin formato (como en el archivo fuente) del campo 'Duration Type' de la actividad. |
| [getRawStatus()](#getRawStatus--) | Obtiene la representación de texto sin formato (como en el archivo fuente) del campo 'Status' de la actividad. |
| [getRemainingEarlyFinish()](#getRemainingEarlyFinish--) | Obtiene la fecha de finalización anticipada restante - la fecha en que se programa que el trabajo restante de la actividad se termine. |
| [getRemainingEarlyStart()](#getRemainingEarlyStart--) | Obtiene la fecha de inicio anticipado restante - la fecha en que se programa que el trabajo restante de la actividad comience. |
| [getRemainingExpenseCost()](#getRemainingExpenseCost--) | Obtiene el valor del costo de gasto restante. |
| [getRemainingLaborUnits()](#getRemainingLaborUnits--) | Obtiene el valor de las unidades de mano de obra restantes. |
| [getRemainingLateFinish()](#getRemainingLateFinish--) | Obtiene la fecha de finalización tardía restante. |
| [getRemainingLateStart()](#getRemainingLateStart--) | Obtiene la fecha de inicio tardío restante. |
| [getRemainingNonLaborUnits()](#getRemainingNonLaborUnits--) | Obtiene el valor de las unidades no laborales restantes. |
| [getSecondaryConstraintDate()](#getSecondaryConstraintDate--) | Obtiene la fecha de la restricción secundaria. |
| [getSecondaryConstraintType()](#getSecondaryConstraintType--) | Obtiene un tipo de restricción secundaria. |
| [getSequenceNumber()](#getSequenceNumber--) | Obtiene el número de secuencia del elemento WBS (tareas resumen). |
| [getUnitsPercentComplete()](#getUnitsPercentComplete--) | Obtiene el valor del porcentaje de unidades completado. |
### getActivityId() {#getActivityId--}
```
public final String getActivityId()
```


Obtiene un campo de id de actividad - el identificador único de la tarea utilizado por Primavera.

--------------------

Aplicable solo a actividades (tareas no resumidas).

**Returns:**
java.lang.String - un campo de id de actividad - el identificador único de una tarea usado por Primavera.
### getActivityType() {#getActivityType--}
```
public final int getActivityType()
```


Obtiene el valor del campo 'Activity Type'.

--------------------

Aplicable solo a actividades (tareas no resumidas).

**Returns:**
int - el valor del campo 'Activity Type'.
### getActualExpenseCost() {#getActualExpenseCost--}
```
public final BigDecimal getActualExpenseCost()
```


Obtiene el valor del costo real del gasto.

**Returns:**
java.math.BigDecimal - el valor del costo real de gasto.
### getActualLaborCost() {#getActualLaborCost--}
```
public final BigDecimal getActualLaborCost()
```


Obtiene el valor del costo laboral real.

**Returns:**
java.math.BigDecimal - el valor del costo real de mano de obra.
### getActualLaborUnits() {#getActualLaborUnits--}
```
public final double getActualLaborUnits()
```


Obtiene el valor de las unidades laborales reales.

**Returns:**
double - el valor de las unidades reales de mano de obra.
### getActualMaterialCost() {#getActualMaterialCost--}
```
public final BigDecimal getActualMaterialCost()
```


Obtiene el valor del costo material real.

**Returns:**
java.math.BigDecimal - el valor del costo real de material.
### getActualNonLaborUnits() {#getActualNonLaborUnits--}
```
public final double getActualNonLaborUnits()
```


Obtiene el valor de las unidades no laborales reales.

**Returns:**
double - el valor de las unidades reales no laborales.
### getActualNonlaborCost() {#getActualNonlaborCost--}
```
public final BigDecimal getActualNonlaborCost()
```


Obtiene el valor del costo no laboral real.

**Returns:**
java.math.BigDecimal - el valor del costo real no laboral.
### getActualTotalCost() {#getActualTotalCost--}
```
public final BigDecimal getActualTotalCost()
```


Obtiene el valor total de los costos reales.

**Returns:**
java.math.BigDecimal - el valor total de los costos reales.
### getBudgetedExpenseCost() {#getBudgetedExpenseCost--}
```
public final BigDecimal getBudgetedExpenseCost()
```


Obtiene el valor del costo presupuestado (o planificado) de gastos.

**Returns:**
java.math.BigDecimal - el valor del costo presupuestado (o planificado) de gasto.
### getBudgetedLaborCost() {#getBudgetedLaborCost--}
```
public final BigDecimal getBudgetedLaborCost()
```


Obtiene el valor del costo laboral presupuestado (o planificado).

**Returns:**
java.math.BigDecimal - el valor del costo presupuestado (o planificado) de mano de obra.
### getBudgetedMaterialCost() {#getBudgetedMaterialCost--}
```
public final BigDecimal getBudgetedMaterialCost()
```


Obtiene el valor del costo material presupuestado (o planificado).

**Returns:**
java.math.BigDecimal - el valor del costo presupuestado (o planificado) de material.
### getBudgetedNonlaborCost() {#getBudgetedNonlaborCost--}
```
public final BigDecimal getBudgetedNonlaborCost()
```


Obtiene el valor del costo no laboral presupuestado (o planificado).

**Returns:**
java.math.BigDecimal - el valor del costo presupuestado (o planificado) no laboral.
### getBudgetedTotalCost() {#getBudgetedTotalCost--}
```
public final BigDecimal getBudgetedTotalCost()
```


Obtiene el valor total de los costos presupuestados (o planificados).

**Returns:**
java.math.BigDecimal - el valor total de los costos presupuestados (o planificados).
### getDurationPercentComplete() {#getDurationPercentComplete--}
```
public final double getDurationPercentComplete()
```


Obtiene el valor del porcentaje completado de la duración.

**Returns:**
double - el valor del porcentaje de duración completado.
### getDurationType() {#getDurationType--}
```
public final int getDurationType()
```


Obtiene el valor del campo 'Duration Type' de la actividad.

--------------------

Aplicable solo a actividades (tareas no resumidas).

**Returns:**
int - el valor del campo 'Duration Type' de la actividad.
### getPercentCompleteType() {#getPercentCompleteType--}
```
public final int getPercentCompleteType()
```


Obtiene el valor del campo '% Complete Type' de la actividad.

--------------------

Aplicable solo a actividades (tareas no resumidas).

**Returns:**
int - el valor del campo '% Complete Type' de la actividad.
### getPhysicalPercentComplete() {#getPhysicalPercentComplete--}
```
public final double getPhysicalPercentComplete()
```


Obtiene el valor de Physical Percent Complete.

--------------------

Aplicable solo a actividades (tareas no resumidas).

**Returns:**
double - el valor de Physical Percent Complete.
### getPlannedDuration() {#getPlannedDuration--}
```
public final Duration getPlannedDuration()
```


Obtiene la duración original o planificada -- el tiempo total de trabajo desde la fecha de inicio planificada de la tarea hasta la fecha de finalización planificada.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - the original or planned duration -- the total working time from the task planned start date to the planned finish date.
### getPrimaryConstraintDate() {#getPrimaryConstraintDate--}
```
public final Date getPrimaryConstraintDate()
```


Obtiene la fecha de la restricción primaria.

**Returns:**
java.util.Date - la fecha de la restricción primaria.
### getPrimaryConstraintType() {#getPrimaryConstraintType--}
```
public final int getPrimaryConstraintType()
```


Obtiene un tipo de restricción primaria.

**Returns:**
int - un tipo de restricción primaria.
### getRawActivityType() {#getRawActivityType--}
```
public final String getRawActivityType()
```


Obtiene la representación de texto sin formato (como en el archivo fuente) del campo 'Activity Type' de la actividad.

--------------------

Aplicable solo a actividades (tareas no resumidas).

**Returns:**
java.lang.String - representación de texto sin formato (como en el archivo fuente) del campo 'Activity Type' de la actividad.
### getRawCompletePercentType() {#getRawCompletePercentType--}
```
public final String getRawCompletePercentType()
```


Obtiene la representación de texto sin formato (como en el archivo fuente) del campo '% Complete Type' de la actividad.

--------------------

Aplicable solo a actividades (tareas no resumidas).

**Returns:**
java.lang.String - representación de texto sin formato (como en el archivo fuente) del campo '% Complete Type' de la actividad.
### getRawDurationType() {#getRawDurationType--}
```
public final String getRawDurationType()
```


Obtiene la representación de texto sin formato (como en el archivo fuente) del campo 'Duration Type' de la actividad.

--------------------

Aplicable solo a actividades (tareas no resumidas).

**Returns:**
java.lang.String - representación de texto sin formato (como en el archivo fuente) del campo 'Duration Type' de la actividad.
### getRawStatus() {#getRawStatus--}
```
public final String getRawStatus()
```


Obtiene la representación de texto sin formato (como en el archivo fuente) del campo 'Status' de la actividad.

--------------------

Aplicable solo a actividades (tareas no resumidas).

**Returns:**
java.lang.String - representación de texto sin formato (como en el archivo fuente) del campo 'Status' de la actividad.
### getRemainingEarlyFinish() {#getRemainingEarlyFinish--}
```
public final Date getRemainingEarlyFinish()
```


Obtiene la fecha de finalización anticipada restante - la fecha en que se programa que el trabajo restante de la actividad se termine.

**Returns:**
java.util.Date - fecha de finalización temprana restante - la fecha en que se programa que el trabajo restante de la actividad se termine.
### getRemainingEarlyStart() {#getRemainingEarlyStart--}
```
public final Date getRemainingEarlyStart()
```


Obtiene la fecha de inicio anticipado restante - la fecha en que se programa que el trabajo restante de la actividad comience.

**Returns:**
java.util.Date - fecha de inicio temprano restante - la fecha en que se programa que el trabajo restante de la actividad comience.
### getRemainingExpenseCost() {#getRemainingExpenseCost--}
```
public final BigDecimal getRemainingExpenseCost()
```


Obtiene el valor del costo de gasto restante.

**Returns:**
java.math.BigDecimal - el valor del costo de gasto restante.
### getRemainingLaborUnits() {#getRemainingLaborUnits--}
```
public final double getRemainingLaborUnits()
```


Obtiene el valor de las unidades de mano de obra restantes.

**Returns:**
double - el valor de las unidades de mano de obra restantes.
### getRemainingLateFinish() {#getRemainingLateFinish--}
```
public final Date getRemainingLateFinish()
```


Obtiene la fecha de finalización tardía restante.

**Returns:**
java.util.Date - fecha de finalización tardía restante.
### getRemainingLateStart() {#getRemainingLateStart--}
```
public final Date getRemainingLateStart()
```


Obtiene la fecha de inicio tardío restante.

**Returns:**
java.util.Date - fecha de inicio tardío restante.
### getRemainingNonLaborUnits() {#getRemainingNonLaborUnits--}
```
public final double getRemainingNonLaborUnits()
```


Obtiene el valor de las unidades no laborales restantes.

**Returns:**
double - el valor de las unidades no laborales restantes.
### getSecondaryConstraintDate() {#getSecondaryConstraintDate--}
```
public final Date getSecondaryConstraintDate()
```


Obtiene la fecha de la restricción secundaria.

**Returns:**
java.util.Date - la fecha de la restricción secundaria.
### getSecondaryConstraintType() {#getSecondaryConstraintType--}
```
public final int getSecondaryConstraintType()
```


Obtiene un tipo de restricción secundaria.

**Returns:**
int - un tipo de restricción secundaria.
### getSequenceNumber() {#getSequenceNumber--}
```
public final int getSequenceNumber()
```


Obtiene el número de secuencia del elemento WBS (tareas resumidas). Se utiliza para ordenar las tareas resumidas en Primavera.

--------------------

Aplicable a los elementos WBS (tareas resumidas).

**Returns:**
int - el número de secuencia del elemento WBS (tareas resumidas).
### getUnitsPercentComplete() {#getUnitsPercentComplete--}
```
public final double getUnitsPercentComplete()
```


Obtiene el valor del porcentaje de unidades completado.

**Returns:**
double - el valor del porcentaje completado de unidades.
