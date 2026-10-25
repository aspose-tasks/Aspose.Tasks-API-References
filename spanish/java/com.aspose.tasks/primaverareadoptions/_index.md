---
title: "PrimaveraReadOptions"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Permite especificar opciones adicionales al leer archivos Primavera Xml o Primavera Xer."
type: docs
weight: 206
url: /es/java/com.aspose.tasks/primaverareadoptions/
---

**Inheritance:**
java.lang.Object
```
public class PrimaveraReadOptions
```

Permite especificar opciones adicionales al leer archivos Primavera Xml o Primavera Xer.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [PrimaveraReadOptions()](#PrimaveraReadOptions--) | Inicializa una nueva instancia de la [PrimaveraReadOptions](../../com.aspose/tasks/primaverareadoptions) clase. |
## Métodos

| Método | Descripción |
| --- | --- |
| [getPreserveUids()](#getPreserveUids--) | Obtiene una bandera que especifica si los identificadores únicos originales de las entidades deben preservarse. |
| [getProjectUid()](#getProjectUid--) | Obtiene el UID de un proyecto para leer de un archivo que contiene varios proyectos. |
| [getReadBaselineProjects()](#getReadBaselineProjects--) | Obtiene una bandera que especifica si los proyectos de línea base deben cargarse. |
| [getUndefinedConstraintHandlingBehavior()](#getUndefinedConstraintHandlingBehavior--) | Especifica el comportamiento utilizado para procesar tareas con restricciones indefinidas leídas del formato XER. |
| [setPreserveUids(boolean value)](#setPreserveUids-boolean-) | Establece una bandera que especifica si los identificadores únicos originales de las entidades deben preservarse. |
| [setProjectUid(int value)](#setProjectUid-int-) | Establece el UID de un proyecto para leer de un archivo que contiene varios proyectos. |
| [setReadBaselineProjects(boolean value)](#setReadBaselineProjects-boolean-) | Establece una bandera que especifica si los proyectos de línea base deben cargarse. |
| [setUndefinedConstraintHandlingBehavior(int value)](#setUndefinedConstraintHandlingBehavior-int-) | Especifica el comportamiento utilizado para procesar tareas con restricciones indefinidas leídas del formato XER. |
### PrimaveraReadOptions() {#PrimaveraReadOptions--}
```
public PrimaveraReadOptions()
```


Inicializa una nueva instancia de la [PrimaveraReadOptions](../../com.aspose/tasks/primaverareadoptions) clase.

### getPreserveUids() {#getPreserveUids--}
```
public final boolean getPreserveUids()
```


Obtiene una bandera que especifica si los identificadores únicos originales de las entidades deben preservarse.

**Returns:**
boolean - una bandera que especifica si los identificadores únicos originales de las entidades deben preservarse.
### getProjectUid() {#getProjectUid--}
```
public final int getProjectUid()
```


Obtiene el UID de un proyecto para leer de un archivo que contiene varios proyectos.

**Returns:**
int - el UID de un proyecto para leer de un archivo que contiene varios proyectos.
### getReadBaselineProjects() {#getReadBaselineProjects--}
```
public final boolean getReadBaselineProjects()
```


Obtiene una bandera que especifica si los proyectos de línea base deben cargarse. El valor predeterminado es true.

--------------------

La bandera es aplicable a archivos Primavera XML que contienen proyectos de línea base (las líneas base no son compatibles con el formato XER). La opción puede establecerse en false para acelerar la carga de un proyecto grande con líneas base cuando no se necesitan los datos de línea base.

**Returns:**
boolean - una bandera que especifica si los proyectos de línea base deben cargarse.
### getUndefinedConstraintHandlingBehavior() {#getUndefinedConstraintHandlingBehavior--}
```
public final int getUndefinedConstraintHandlingBehavior()
```


Especifica el comportamiento utilizado para procesar tareas con restricciones indefinidas leídas del formato XER.

**Returns:**
int - el comportamiento utilizado para procesar tareas con restricciones indefinidas leídas del formato XER.
### setPreserveUids(boolean value) {#setPreserveUids-boolean-}
```
public final void setPreserveUids(boolean value)
```


Establece una bandera que especifica si los identificadores únicos originales de las entidades deben preservarse.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean | una bandera que especifica si los identificadores únicos originales de las entidades deben preservarse. |

### setProjectUid(int value) {#setProjectUid-int-}
```
public final void setProjectUid(int value)
```


Establece el UID de un proyecto para leer de un archivo que contiene varios proyectos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | el UID de un proyecto para leer de un archivo que contiene varios proyectos. |

### setReadBaselineProjects(boolean value) {#setReadBaselineProjects-boolean-}
```
public final void setReadBaselineProjects(boolean value)
```


Establece una bandera que especifica si los proyectos de línea base deben cargarse. El valor predeterminado es verdadero.

--------------------

La bandera es aplicable a archivos Primavera XML que contienen proyectos de línea base (las líneas base no son compatibles con el formato XER). La opción puede establecerse en false para acelerar la carga de un proyecto grande con líneas base cuando no se necesitan los datos de línea base.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean | una bandera que especifica si los proyectos de línea base deben cargarse. |

### setUndefinedConstraintHandlingBehavior(int value) {#setUndefinedConstraintHandlingBehavior-int-}
```
public final void setUndefinedConstraintHandlingBehavior(int value)
```


Especifica el comportamiento utilizado para procesar tareas con restricciones indefinidas leídas del formato XER.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | el comportamiento utilizado para procesar tareas con restricciones indefinidas leídas del formato XER. |

