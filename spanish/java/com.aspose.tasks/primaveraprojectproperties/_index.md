---
title: "PrimaveraProjectProperties"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Representa propiedades específicas de Primavera para un proyecto leído de archivos Primavera XER o P6XML."
type: docs
weight: 205
url: /es/java/com.aspose.tasks/primaveraprojectproperties/
---

**Inheritance:**
java.lang.Object
```
public final class PrimaveraProjectProperties
```

Representa propiedades específicas de Primavera para un proyecto leído de archivos Primavera (XER o P6XML).
## Métodos

| Método | Descripción |
| --- | --- |
| [getBaselineProjects()](#getBaselineProjects--) | Obtiene la matriz de proyectos de línea base del proyecto actual. |
| [getCriticalActivitiesDefiningMethod()](#getCriticalActivitiesDefiningMethod--) | Obtiene el método para definir actividades críticas: enfoque de Ruta Más Larga o Flotación Total. |
| [getCriticalTotalFloatLimit()](#getCriticalTotalFloatLimit--) | Obtiene el valor umbral utilizado para definir actividades críticas si se usa el método TotalFloat. |
| [getCurrentBaselineProjectId()](#getCurrentBaselineProjectId--) | Obtiene el Id del proyecto de línea base actual. |
| [getIgnoreOtherProjectRelationships()](#getIgnoreOtherProjectRelationships--) | Obtiene una bandera que define si se deben ignorar las relaciones de actividades entre proyectos. |
| [getMakeOpenEndedActivitiesCritical()](#getMakeOpenEndedActivitiesCritical--) | Obtiene una bandera que define si las actividades deben marcarse como críticas al programar el proyecto. |
| [getRelationshipLagCalendar()](#getRelationshipLagCalendar--) | Obtiene una opción que define qué calendario usar para programar el retraso de relaciones en proyectos Primavera. |
| [getShortName()](#getShortName--) | Obtiene el nombre corto del proyecto (ID del proyecto). |
| [getUseExpectedFinishDates()](#getUseExpectedFinishDates--) | Obtiene una bandera que define si las fechas de finalización de actividades deben programarse como las fechas de finalización esperadas. |
### getBaselineProjects() {#getBaselineProjects--}
```
public final Project[] getBaselineProjects()
```


Obtiene la matriz de proyectos de línea base del proyecto actual. Es aplicable a proyectos leídos de archivos XML de Primavera que contienen líneas base exportadas.

**Returns:**
com.aspose.tasks.Project[] - matriz de proyectos de línea base del proyecto actual.
### getCriticalActivitiesDefiningMethod() {#getCriticalActivitiesDefiningMethod--}
```
public final int getCriticalActivitiesDefiningMethod()
```


Obtiene el método para definir actividades críticas: enfoque de Ruta Más Larga o Flotación Total.

**Returns:**
int - el método para definir actividades críticas: enfoque de Ruta Más Larga o Flotación Total.
### getCriticalTotalFloatLimit() {#getCriticalTotalFloatLimit--}
```
public final Double getCriticalTotalFloatLimit()
```


Obtiene el valor umbral utilizado para definir actividades críticas si se usa el método TotalFloat.

**Returns:**
java.lang.Double - el valor umbral utilizado para definir actividades críticas si se usa el método TotalFloat.
### getCurrentBaselineProjectId() {#getCurrentBaselineProjectId--}
```
public final int getCurrentBaselineProjectId()
```


Obtiene el Id del proyecto de línea base actual. Es aplicable a proyectos leídos de archivos XML de Primavera que contienen líneas base exportadas.

**Returns:**
int - Id del proyecto de línea base actual.
### getIgnoreOtherProjectRelationships() {#getIgnoreOtherProjectRelationships--}
```
public final boolean getIgnoreOtherProjectRelationships()
```


Obtiene una bandera que define si se deben ignorar las relaciones de actividades entre proyectos.

**Returns:**
boolean - una bandera que define si se deben ignorar las relaciones de actividades entre proyectos.
### getMakeOpenEndedActivitiesCritical() {#getMakeOpenEndedActivitiesCritical--}
```
public final boolean getMakeOpenEndedActivitiesCritical()
```


Obtiene una bandera que define si las actividades deben marcarse como críticas al programar el proyecto.

**Returns:**
boolean - una bandera que define si las actividades deben marcarse como críticas al programar el proyecto.
### getRelationshipLagCalendar() {#getRelationshipLagCalendar--}
```
public final int getRelationshipLagCalendar()
```


Obtiene una opción que define qué calendario usar para programar el retraso de relaciones en proyectos Primavera.

**Returns:**
int - una opción que define qué calendario usar para programar el Relationship Lag en proyectos Primavera
### getShortName() {#getShortName--}
```
public final String getShortName()
```


Obtiene el nombre corto del proyecto (ID del proyecto).

**Returns:**
java.lang.String - nombre corto del proyecto (ID del proyecto).
### getUseExpectedFinishDates() {#getUseExpectedFinishDates--}
```
public final boolean getUseExpectedFinishDates()
```


Obtiene una bandera que define si las fechas de finalización de actividades deben programarse como las fechas de finalización esperadas.

**Returns:**
boolean - una bandera que define si las fechas de finalización de actividades deben programarse como las fechas de finalización esperadas.
