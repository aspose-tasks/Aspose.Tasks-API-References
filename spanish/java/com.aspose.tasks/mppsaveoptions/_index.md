---
title: "MPPSaveOptions"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Permite especificar opciones adicionales al guardar datos del proyecto en MPP."
type: docs
weight: 149
url: /es/java/com.aspose.tasks/mppsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions)
```
public class MPPSaveOptions extends SimpleSaveOptions
```

Permite especificar opciones adicionales al guardar datos del proyecto en MPP.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [MPPSaveOptions()](#MPPSaveOptions--) | Inicializa una nueva instancia de la clase [MPPSaveOptions](../../com.aspose.tasks/mppsaveoptions). |
## Métodos

| Método | Descripción |
| --- | --- |
| [getClearVba()](#getClearVba--) | Obtiene un valor que indica si se deben eliminar los datos de macros VBA existentes al guardar un proyecto en formato MPP. |
| [getProtectionPassword()](#getProtectionPassword--) | Obtiene una contraseña que se utiliza para proteger el archivo MPP resultante. |
| [getRemoveInvalidAssignments()](#getRemoveInvalidAssignments--) | Obtiene un valor que indica si se deben eliminar asignaciones de recursos no válidas al guardar en MPP. |
| [getWriteFilters()](#getWriteFilters--) | Obtiene un valor que indica si se deben escribir datos de filtro al guardar un proyecto en MPP para el formato. |
| [getWriteGroups()](#getWriteGroups--) | Obtiene un valor que indica si se deben escribir los datos de grupos al guardar un proyecto en formato MPP. |
| [getWriteVba()](#getWriteVba--) | Obtiene un valor que indica si se deben actualizar los datos de macros VBA existentes en el archivo MPP. |
| [getWriteViewData()](#getWriteViewData--) | Obtiene un valor que indica si se deben escribir los datos de vista al guardar un proyecto en formato MPP. |
| [setClearVba(boolean value)](#setClearVba-boolean-) | Establece un valor que indica si se deben eliminar los datos de macros VBA existentes al guardar un proyecto en formato MPP. |
| [setProtectionPassword(String value)](#setProtectionPassword-java.lang.String-) | Establece una contraseña que se utiliza para proteger el archivo MPP resultante. |
| [setRemoveInvalidAssignments(boolean value)](#setRemoveInvalidAssignments-boolean-) | Establece un valor que indica si se deben eliminar asignaciones de recursos inválidas al guardar en MPP. |
| [setWriteFilters(boolean value)](#setWriteFilters-boolean-) | Establece un valor que indica si se deben escribir los datos de filtro al guardar un proyecto en formato MPP. |
| [setWriteGroups(boolean value)](#setWriteGroups-boolean-) | Establece un valor que indica si se deben escribir los datos de grupos al guardar un proyecto en formato MPP. |
| [setWriteVba(boolean value)](#setWriteVba-boolean-) | Establece un valor que indica si se deben actualizar los datos de macros VBA existentes en el archivo MPP. |
| [setWriteViewData(boolean value)](#setWriteViewData-boolean-) | Establece un valor que indica si se deben escribir los datos de vista al guardar un proyecto en formato MPP. |
### MPPSaveOptions() {#MPPSaveOptions--}
```
public MPPSaveOptions()
```


Inicializa una nueva instancia de la clase [MPPSaveOptions](../../com.aspose.tasks/mppsaveoptions).

### getClearVba() {#getClearVba--}
```
public final boolean getClearVba()
```


Obtiene un valor que indica si se deben eliminar los datos de macros VBA existentes al guardar un proyecto en formato MPP.

**Returns:**
boolean - un valor que indica si se deben eliminar los datos de macros VBA existentes al guardar un proyecto en formato MPP.
### getProtectionPassword() {#getProtectionPassword--}
```
public final String getProtectionPassword()
```


Obtiene una contraseña que se utiliza para proteger el archivo MPP resultante. Actualmente es compatible con MS Project 2010 y formatos posteriores.

--------------------

Un valor nulo indica que el archivo del proyecto no está protegido.

**Returns:**
java.lang.String - una contraseña que se utiliza para proteger el archivo MPP resultante.
### getRemoveInvalidAssignments() {#getRemoveInvalidAssignments--}
```
public final boolean getRemoveInvalidAssignments()
```


Obtiene un valor que indica si se deben eliminar asignaciones de recursos no válidas al guardar en MPP.

--------------------

MS Project crea una asignación de recurso vacía para cada tarea. Establezca este indicador en true para eliminarlas al guardar.

**Returns:**
boolean - un valor que indica si se deben eliminar asignaciones de recursos inválidas al guardar en MPP.
### getWriteFilters() {#getWriteFilters--}
```
public final boolean getWriteFilters()
```


Obtiene un valor que indica si se deben escribir datos de filtro al guardar un proyecto en MPP para el formato.

--------------------

Los datos de filtro incluyen las colecciones Project.TaskFilters y Project.ResourceFilters.

--------------------

Actualmente compatible con MSP 2010 o formatos posteriores.

**Returns:**
boolean - un valor que indica si se deben escribir los datos de filtro al guardar un proyecto en formato MPP.
### getWriteGroups() {#getWriteGroups--}
```
public final boolean getWriteGroups()
```


Obtiene un valor que indica si se deben escribir los datos de grupos al guardar un proyecto en formato MPP.

--------------------

Los datos de grupo incluyen las colecciones Project.TaskGroups y Project.ResourceGroups.

**Returns:**
boolean - un valor que indica si se deben escribir los datos de grupos al guardar un proyecto en formato MPP.
### getWriteVba() {#getWriteVba--}
```
public final boolean getWriteVba()
```


Obtiene un valor que indica si se deben actualizar los datos de macros VBA existentes en el archivo MPP. Actualmente se admite la escritura de VbaModule.SourceCode.

**Returns:**
boolean - un valor que indica si se deben actualizar los datos de macros VBA existentes en el archivo MPP.
### getWriteViewData() {#getWriteViewData--}
```
public final boolean getWriteViewData()
```


Obtiene un valor que indica si se deben escribir los datos de vista al guardar un proyecto en formato MPP.

--------------------

Los datos de vista incluyen las colecciones Project.Views, Filters y Tables.

**Returns:**
boolean - un valor que indica si se deben escribir los datos de vista al guardar un proyecto en formato MPP.
### setClearVba(boolean value) {#setClearVba-boolean-}
```
public final void setClearVba(boolean value)
```


Establece un valor que indica si se deben eliminar los datos de macros VBA existentes al guardar un proyecto en formato MPP.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean | un valor que indica si se debe eliminar los datos de macros VBA existentes al guardar un proyecto en formato MPP. |

### setProtectionPassword(String value) {#setProtectionPassword-java.lang.String-}
```
public final void setProtectionPassword(String value)
```


Establece una contraseña que se utiliza para proteger un archivo MPP resultante. Actualmente es compatible con MS Project 2010 y formatos más recientes.

--------------------

Un valor nulo indica que el archivo del proyecto no está protegido.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String | una contraseña que se utiliza para proteger un archivo MPP resultante. |

### setRemoveInvalidAssignments(boolean value) {#setRemoveInvalidAssignments-boolean-}
```
public final void setRemoveInvalidAssignments(boolean value)
```


Establece un valor que indica si se deben eliminar asignaciones de recursos inválidas al guardar en MPP.

--------------------

MS Project crea una asignación de recurso vacía para cada tarea. Establezca este indicador en true para eliminarlas al guardar.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean | un valor que indica si se deben eliminar asignaciones de recursos inválidas al guardar en MPP. |

### setWriteFilters(boolean value) {#setWriteFilters-boolean-}
```
public final void setWriteFilters(boolean value)
```


Establece un valor que indica si se deben escribir los datos de filtro al guardar un proyecto en formato MPP.

--------------------

Los datos de filtro incluyen las colecciones Project.TaskFilters y Project.ResourceFilters.

--------------------

Actualmente compatible con MSP 2010 o formatos posteriores.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean | un valor que indica si se deben escribir datos de filtros al guardar un proyecto en formato MPP. |

### setWriteGroups(boolean value) {#setWriteGroups-boolean-}
```
public final void setWriteGroups(boolean value)
```


Establece un valor que indica si se deben escribir los datos de grupos al guardar un proyecto en formato MPP.

--------------------

Los datos de grupo incluyen las colecciones Project.TaskGroups y Project.ResourceGroups.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean | un valor que indica si se deben escribir datos de grupos al guardar un proyecto en formato MPP. |

### setWriteVba(boolean value) {#setWriteVba-boolean-}
```
public final void setWriteVba(boolean value)
```


Establece un valor que indica si se deben actualizar los datos de macros VBA existentes en el archivo MPP. Actualmente se admite la escritura de VbaModule.SourceCode.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean | un valor que indica si se deben actualizar los datos de macros VBA existentes en el archivo MPP. |

### setWriteViewData(boolean value) {#setWriteViewData-boolean-}
```
public final void setWriteViewData(boolean value)
```


Establece un valor que indica si se deben escribir los datos de vista al guardar un proyecto en formato MPP.

--------------------

Los datos de vista incluyen las colecciones Project.Views, Filters y Tables.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean | un valor que indica si se deben escribir datos de vista al guardar un proyecto en formato MPP. |

