---
title: "ResourceLeveler"
second_title: "Aspose.Tasks for Java API-referens"
description: "Innehåller metoder för resursutjämning."
type: docs
weight: 253
url: /sv/java/com.aspose.tasks/resourceleveler/
---

**Inheritance:**
java.lang.Object
```
public class ResourceLeveler
```

Innehåller metoder för resursutjämning.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [ResourceLeveler()](#ResourceLeveler--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [clearLeveling(Project project)](#clearLeveling-com.aspose.tasks.Project-) | Rensar alla nivåfördröjningar som tidigare lagts till projektet under resurshantering. |
| [clearLeveling(Iterable&lt;Task&gt; tasks)](#clearLeveling-java.lang.Iterable-com.aspose.tasks.Task--) | Rensar alla nivåfördröjningar som tidigare lagts till de angivna uppgifterna under resurshantering. |
| [levelAll(Project project)](#levelAll-com.aspose.tasks.Project-) | Nivåinställer uppgifter för alla projektets resurser med standardnivåalternativ. |
| [levelResources(Project project, LevelingOptions options)](#levelResources-com.aspose.tasks.Project-com.aspose.tasks.LevelingOptions-) | Nivåinställer uppgifter för de angivna resurserna med de angivna nivåalternativen. |
### ResourceLeveler() {#ResourceLeveler--}
```
public ResourceLeveler()
```


### clearLeveling(Project project) {#clearLeveling-com.aspose.tasks.Project-}
```
public static void clearLeveling(Project project)
```


Rensar alla nivåfördröjningar som tidigare lagts till projektet under resurshantering.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| project | [Project](../../com.aspose.tasks/project) | Projekt för att rensa nivåinställning. |

### clearLeveling(Iterable&lt;Task&gt; tasks) {#clearLeveling-java.lang.Iterable-com.aspose.tasks.Task--}
```
public static void clearLeveling(Iterable<Task> tasks)
```


Rensar alla nivåfördröjningar som tidigare lagts till de angivna uppgifterna under resurshantering.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| uppgifter | java.lang.Iterable&lt;com.aspose.tasks.Task&gt; | Den uppräkningsbara som innehåller uppgifter vars nivåfördröjning ska rensas. |

### levelAll(Project project) {#levelAll-com.aspose.tasks.Project-}
```
public static LevelingResult levelAll(Project project)
```


Nivåinställer uppgifter för alla projektets resurser med standardnivåalternativ.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| project | [Project](../../com.aspose.tasks/project) | Projekt för att tillämpa resurshantering. |

**Returns:**
[LevelingResult](../../com.aspose.tasks/levelingresult) - Object containing results of resource leveling.
### levelResources(Project project, LevelingOptions options) {#levelResources-com.aspose.tasks.Project-com.aspose.tasks.LevelingOptions-}
```
public static LevelingResult levelResources(Project project, LevelingOptions options)
```


Nivåinställer uppgifter för de angivna resurserna med de angivna nivåalternativen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| project | [Project](../../com.aspose.tasks/project) | Projekt för att tillämpa resurshantering. |
| options | [LevelingOptions](../../com.aspose.tasks/levelingoptions) | Alternativ som specificerar hur resurser ska nivåinställas. |

**Returns:**
[LevelingResult](../../com.aspose.tasks/levelingresult) - Object containing results of resource leveling.
