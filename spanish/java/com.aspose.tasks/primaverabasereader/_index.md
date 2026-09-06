---
title: "PrimaveraBaseReader"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Representa un lector base que puede usarse para leer los UID del proyecto de archivos Primavera XER o XML de múltiples proyectos."
type: docs
weight: 196
url: /es/java/com.aspose.tasks/primaverabasereader/
---

**Inheritance:**
java.lang.Object
```
public abstract class PrimaveraBaseReader
```

Representa un lector base que puede usarse para leer los UID del proyecto de archivos Primavera XER o XML de múltiples proyectos.
## Métodos

| Método | Descripción |
| --- | --- |
| [getProjectInfos()](#getProjectInfos--) | Devuelve una lista de los objetos de información breve del proyecto. |
| [getProjectUids()](#getProjectUids--) | Devuelve una lista de los identificadores únicos de los proyectos. |
| [loadProject(int projectUid)](#loadProject-int-) | Carga el proyecto con el identificador único especificado. |
### getProjectInfos() {#getProjectInfos--}
```
public final List<PrimaveraProjectInfo> getProjectInfos()
```


Devuelve una lista de los objetos de información breve del proyecto.

**Returns:**
java.util.List&lt;com.aspose.tasks.PrimaveraProjectInfo&gt; - una lista de los objetos de información breve del proyecto
### getProjectUids() {#getProjectUids--}
```
public final List<Integer> getProjectUids()
```


Devuelve una lista de los identificadores únicos de los proyectos.

**Returns:**
java.util.List&lt;java.lang.Integer&gt; - Lista de los identificadores únicos de los proyectos.
### loadProject(int projectUid) {#loadProject-int-}
```
public Project loadProject(int projectUid)
```


Carga el proyecto con el identificador único especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| projectUid | int | Identificador único del proyecto a cargar. |

**Returns:**
[Project](../../com.aspose.tasks/project) - Project with specified unique identifier from the specified multi project file. Null if project doesn't exist.
