---
title: "ResourceLeveler"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Contiene métodos de nivelación de recursos."
type: docs
weight: 253
url: /es/java/com.aspose.tasks/resourceleveler/
---

**Inheritance:**
java.lang.Object
```
public class ResourceLeveler
```

Contiene métodos de nivelación de recursos.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [ResourceLeveler()](#ResourceLeveler--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
| [clearLeveling(Project project)](#clearLeveling-com.aspose.tasks.Project-) | Elimina cualquier retraso de nivelación que se haya añadido previamente al proyecto durante la nivelación de recursos. |
| [clearLeveling(Iterable&lt;Task&gt; tasks)](#clearLeveling-java.lang.Iterable-com.aspose.tasks.Task--) | Elimina cualquier retraso de nivelación que se haya añadido previamente a las tareas especificadas durante la nivelación de recursos. |
| [levelAll(Project project)](#levelAll-com.aspose.tasks.Project-) | Niveliza las tareas para todos los recursos del proyecto usando las opciones de nivelación predeterminadas. |
| [levelResources(Project project, LevelingOptions options)](#levelResources-com.aspose.tasks.Project-com.aspose.tasks.LevelingOptions-) | Niveliza las tareas para los recursos especificados usando las opciones de nivelación especificadas. |
### ResourceLeveler() {#ResourceLeveler--}
```
public ResourceLeveler()
```


### clearLeveling(Project project) {#clearLeveling-com.aspose.tasks.Project-}
```
public static void clearLeveling(Project project)
```


Elimina cualquier retraso de nivelación que se haya añadido previamente al proyecto durante la nivelación de recursos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| project | [Project](../../com.aspose.tasks/project) | Proyecto para eliminar la nivelación. |

### clearLeveling(Iterable&lt;Task&gt; tasks) {#clearLeveling-java.lang.Iterable-com.aspose.tasks.Task--}
```
public static void clearLeveling(Iterable<Task> tasks)
```


Elimina cualquier retraso de nivelación que se haya añadido previamente a las tareas especificadas durante la nivelación de recursos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| tareas | java.lang.Iterable&lt;com.aspose.tasks.Task&gt; | El enumerable que contiene las tareas para las que se debe eliminar el retraso de nivelación. |

### levelAll(Project project) {#levelAll-com.aspose.tasks.Project-}
```
public static LevelingResult levelAll(Project project)
```


Niveliza las tareas para todos los recursos del proyecto usando las opciones de nivelación predeterminadas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| project | [Project](../../com.aspose.tasks/project) | Proyecto para aplicar la nivelación de recursos. |

**Returns:**
[LevelingResult](../../com.aspose.tasks/levelingresult) - Object containing results of resource leveling.
### levelResources(Project project, LevelingOptions options) {#levelResources-com.aspose.tasks.Project-com.aspose.tasks.LevelingOptions-}
```
public static LevelingResult levelResources(Project project, LevelingOptions options)
```


Niveliza las tareas para los recursos especificados usando las opciones de nivelación especificadas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| project | [Project](../../com.aspose.tasks/project) | Proyecto para aplicar la nivelación de recursos. |
| options | [LevelingOptions](../../com.aspose.tasks/levelingoptions) | Opciones que especifican cómo nivelar los recursos. |

**Returns:**
[LevelingResult](../../com.aspose.tasks/levelingresult) - Object containing results of resource leveling.
