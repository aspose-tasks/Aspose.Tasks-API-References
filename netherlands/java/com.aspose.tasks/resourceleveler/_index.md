---
title: "ResourceLeveler"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Bevat methoden voor resource-leveling."
type: docs
weight: 253
url: /nl/java/com.aspose.tasks/resourceleveler/
---

**Inheritance:**
java.lang.Object
```
public class ResourceLeveler
```

Bevat methoden voor resource-leveling.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [ResourceLeveler()](#ResourceLeveler--) |  |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [clearLeveling(Project project)](#clearLeveling-com.aspose.tasks.Project-) | Verwijdert elke levelingsvertraging die eerder aan het project is toegevoegd tijdens resource-leveling. |
| [clearLeveling(Iterable&lt;Task&gt; tasks)](#clearLeveling-java.lang.Iterable-com.aspose.tasks.Task--) | Verwijdert elke levelingsvertraging die eerder aan de opgegeven taken is toegevoegd tijdens resource-leveling. |
| [levelAll(Project project)](#levelAll-com.aspose.tasks.Project-) | Levelt taken voor alle resources van het project met behulp van de standaard levelingsopties. |
| [levelResources(Project project, LevelingOptions options)](#levelResources-com.aspose.tasks.Project-com.aspose.tasks.LevelingOptions-) | Levelt taken voor de opgegeven resources met behulp van de opgegeven levelingsopties. |
### ResourceLeveler() {#ResourceLeveler--}
```
public ResourceLeveler()
```


### clearLeveling(Project project) {#clearLeveling-com.aspose.tasks.Project-}
```
public static void clearLeveling(Project project)
```


Verwijdert elke levelingsvertraging die eerder aan het project is toegevoegd tijdens resource-leveling.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| project | [Project](../../com.aspose.tasks/project) | Project om levelings te wissen. |

### clearLeveling(Iterable&lt;Task&gt; tasks) {#clearLeveling-java.lang.Iterable-com.aspose.tasks.Task--}
```
public static void clearLeveling(Iterable<Task> tasks)
```


Verwijdert elke levelingsvertraging die eerder aan de opgegeven taken is toegevoegd tijdens resource-leveling.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| taken | java.lang.Iterable&lt;com.aspose.tasks.Task&gt; | De enumerable die taken bevat waarvoor de levelingsvertraging moet worden gewist. |

### levelAll(Project project) {#levelAll-com.aspose.tasks.Project-}
```
public static LevelingResult levelAll(Project project)
```


Levelt taken voor alle resources van het project met behulp van de standaard levelingsopties.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| project | [Project](../../com.aspose.tasks/project) | Project om resource-leveling toe te passen. |

**Returns:**
[LevelingResult](../../com.aspose.tasks/levelingresult) - Object containing results of resource leveling.
### levelResources(Project project, LevelingOptions options) {#levelResources-com.aspose.tasks.Project-com.aspose.tasks.LevelingOptions-}
```
public static LevelingResult levelResources(Project project, LevelingOptions options)
```


Levelt taken voor de opgegeven resources met behulp van de opgegeven levelingsopties.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| project | [Project](../../com.aspose.tasks/project) | Project om resource-leveling toe te passen. |
| options | [LevelingOptions](../../com.aspose.tasks/levelingoptions) | Opties die specificeren hoe resources moeten worden genivelleerd. |

**Returns:**
[LevelingResult](../../com.aspose.tasks/levelingresult) - Object containing results of resource leveling.
