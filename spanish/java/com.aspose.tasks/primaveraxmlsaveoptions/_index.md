---
title: "PrimaveraXmlSaveOptions"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Permite especificar opciones adicionales al guardar el proyecto en formato Primavera xml."
type: docs
weight: 212
url: /es/java/com.aspose.tasks/primaveraxmlsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions)
```
public class PrimaveraXmlSaveOptions extends SimpleSaveOptions
```

Permite especificar opciones adicionales al guardar el proyecto en formato Primavera xml.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [PrimaveraXmlSaveOptions()](#PrimaveraXmlSaveOptions--) | Inicializa una nueva instancia de la clase [PrimaveraXmlSaveOptions](../../com.aspose.tasks/primaveraxmlsaveoptions). |
## Métodos

| Método | Descripción |
| --- | --- |
| [getSaveRootTask()](#getSaveRootTask--) | Obtiene un valor que indica si se debe guardar una tarea raíz o no. |
| [getSkipSummaryAssignments()](#getSkipSummaryAssignments--) | Obtiene un valor que indica si las asignaciones de recursos a tareas resumen deben omitirse durante la exportación. |
| [setSaveRootTask(boolean value)](#setSaveRootTask-boolean-) | Establece un valor que indica si se debe guardar una tarea raíz o no. |
| [setSkipSummaryAssignments(boolean value)](#setSkipSummaryAssignments-boolean-) | Establece un valor que indica si las asignaciones de recursos a tareas resumen deben omitirse durante la exportación. |
### PrimaveraXmlSaveOptions() {#PrimaveraXmlSaveOptions--}
```
public PrimaveraXmlSaveOptions()
```


Inicializa una nueva instancia de la clase [PrimaveraXmlSaveOptions](../../com.aspose.tasks/primaveraxmlsaveoptions).

### getSaveRootTask() {#getSaveRootTask--}
```
public final boolean getSaveRootTask()
```


Obtiene un valor que indica si se debe guardar una tarea raíz o no.

**Returns:**
boolean - un valor que indica si se debe guardar una tarea raíz o no.
### getSkipSummaryAssignments() {#getSkipSummaryAssignments--}
```
public final boolean getSkipSummaryAssignments()
```


Obtiene un valor que indica si las asignaciones de recursos a tareas resumen deben omitirse durante la exportación.

El software Primavera no admite asignaciones de recursos a tareas resumen (WBS). Por lo tanto, la exportación de dichas asignaciones puede generar un archivo no válido según el modelo de Primavera. Si es true, las asignaciones a tareas resumen se omiten durante la exportación. Si es false (el valor predeterminado), se lanzará una excepción si se encuentra una asignación a una tarea resumen durante la exportación.

**Returns:**
boolean - un valor que indica si las asignaciones de recursos a tareas resumen deben omitirse durante la exportación.
### setSaveRootTask(boolean value) {#setSaveRootTask-boolean-}
```
public final void setSaveRootTask(boolean value)
```


Establece un valor que indica si se debe guardar una tarea raíz o no.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean | un valor que indica si se debe guardar una tarea raíz o no. |

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

