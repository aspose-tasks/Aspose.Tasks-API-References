---
title: "PrimaveraSaveOptions"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Permite especificar opciones adicionales al guardar el proyecto en formato Primavera XER."
type: docs
weight: 208
url: /es/java/com.aspose.tasks/primaverasaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions)
```
public class PrimaveraSaveOptions extends SimpleSaveOptions
```

Permite especificar opciones adicionales al guardar el proyecto en formato Primavera XER.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [PrimaveraSaveOptions()](#PrimaveraSaveOptions--) | Inicializa una nueva instancia de la clase [PrimaveraSaveOptions](../../com.aspose.tasks/primaverasaveoptions). |
## Métodos

| Método | Descripción |
| --- | --- |
| [getActivityIdIncrement()](#getActivityIdIncrement--) | Obtiene el incremento usado al renumerar los IDs de actividad. |
| [getActivityIdPrefix()](#getActivityIdPrefix--) | Obtiene el prefijo usado al renumerar los IDs de actividad. |
| [getActivityIdSuffix()](#getActivityIdSuffix--) | Obtiene el sufijo usado al renumerar los IDs de actividad. |
| [getRenumberActivityIds()](#getRenumberActivityIds--) | Obtiene un valor que indica si es necesario renumerar los IDs de actividad. |
| [getSkipSummaryAssignments()](#getSkipSummaryAssignments--) | Obtiene un valor que indica si las asignaciones de recursos a tareas resumen deben omitirse durante la exportación. |
| [setActivityIdIncrement(int value)](#setActivityIdIncrement-int-) | Establece el incremento usado al renumerar los IDs de actividad. |
| [setActivityIdPrefix(String value)](#setActivityIdPrefix-java.lang.String-) | Establece el prefijo usado al renumerar los IDs de actividad. |
| [setActivityIdSuffix(int value)](#setActivityIdSuffix-int-) | Establece el sufijo usado al renumerar los IDs de actividad. |
| [setRenumberActivityIds(boolean value)](#setRenumberActivityIds-boolean-) | Establece un valor que indica si es necesario renumerar los IDs de actividad. |
| [setSkipSummaryAssignments(boolean value)](#setSkipSummaryAssignments-boolean-) | Establece un valor que indica si las asignaciones de recursos a tareas resumen deben omitirse durante la exportación. |
### PrimaveraSaveOptions() {#PrimaveraSaveOptions--}
```
public PrimaveraSaveOptions()
```


Inicializa una nueva instancia de la clase [PrimaveraSaveOptions](../../com.aspose.tasks/primaverasaveoptions).

### getActivityIdIncrement() {#getActivityIdIncrement--}
```
public final int getActivityIdIncrement()
```


Obtiene el incremento usado al renumerar los IDs de actividad.

**Returns:**
int - el incremento usado en la renumeración de los IDs de actividad.
### getActivityIdPrefix() {#getActivityIdPrefix--}
```
public final String getActivityIdPrefix()
```


Obtiene el prefijo usado al renumerar los IDs de actividad.

**Returns:**
java.lang.String - el prefijo usado en la renumeración de los IDs de actividad.
### getActivityIdSuffix() {#getActivityIdSuffix--}
```
public final int getActivityIdSuffix()
```


Obtiene el sufijo usado al renumerar los IDs de actividad.

**Returns:**
int - el sufijo usado en la renumeración de los IDs de actividad.
### getRenumberActivityIds() {#getRenumberActivityIds--}
```
public final boolean getRenumberActivityIds()
```


Obtiene un valor que indica si es necesario renumerar los IDs de actividad.

**Returns:**
boolean - un valor que indica si es necesario renumerar los IDs de actividad.
### getSkipSummaryAssignments() {#getSkipSummaryAssignments--}
```
public final boolean getSkipSummaryAssignments()
```


Obtiene un valor que indica si las asignaciones de recursos a tareas resumen deben omitirse durante la exportación.

El software Primavera no admite asignaciones de recursos a tareas resumen (WBS). Por lo tanto, la exportación de dichas asignaciones puede generar un archivo no válido según el modelo de Primavera. Si es true, las asignaciones a tareas resumen se omiten durante la exportación. Si es false (el valor predeterminado), se lanzará una excepción si se encuentra una asignación a una tarea resumen durante la exportación.

**Returns:**
boolean - un valor que indica si las asignaciones de recursos a tareas resumen deben omitirse durante la exportación.
### setActivityIdIncrement(int value) {#setActivityIdIncrement-int-}
```
public final void setActivityIdIncrement(int value)
```


Establece el incremento usado al renumerar los IDs de actividad.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | el incremento usado en la renumeración de los IDs de actividad. |

### setActivityIdPrefix(String value) {#setActivityIdPrefix-java.lang.String-}
```
public final void setActivityIdPrefix(String value)
```


Establece el prefijo usado al renumerar los IDs de actividad.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String | el prefijo usado en la renumeración de los IDs de actividad. |

### setActivityIdSuffix(int value) {#setActivityIdSuffix-int-}
```
public final void setActivityIdSuffix(int value)
```


Establece el sufijo usado al renumerar los IDs de actividad.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | el sufijo usado en la renumeración de los IDs de actividad. |

### setRenumberActivityIds(boolean value) {#setRenumberActivityIds-boolean-}
```
public final void setRenumberActivityIds(boolean value)
```


Establece un valor que indica si es necesario renumerar los IDs de actividad.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean | un valor que indica si es necesario renumerar los IDs de actividad. |

### setSkipSummaryAssignments(boolean value) {#setSkipSummaryAssignments-boolean-}
```
public final void setSkipSummaryAssignments(boolean value)
```


Establece un valor que indica si las asignaciones de recursos a tareas resumen deben omitirse durante la exportación.

El software Primavera no admite asignaciones de recursos a tareas resumen (WBS). Por lo tanto, la exportación de dichas asignaciones puede generar un archivo no válido según el modelo de Primavera. Si es true, las asignaciones a tareas resumen se omiten durante la exportación. Si es false (el valor predeterminado), se lanzará una excepción si se encuentra una asignación a una tarea resumen durante la exportación.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean | un valor que indica si las asignaciones de recursos a tareas resumen deben omitirse durante la exportación. |

