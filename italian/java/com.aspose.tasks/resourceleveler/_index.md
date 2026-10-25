---
title: "ResourceLeveler"
second_title: "Aspose.Tasks for Java API Reference"
description: "Contiene metodi di livellamento delle risorse."
type: docs
weight: 253
url: /it/java/com.aspose.tasks/resourceleveler/
---

**Inheritance:**
java.lang.Object
```
public class ResourceLeveler
```

Contiene metodi di livellamento delle risorse.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [ResourceLeveler()](#ResourceLeveler--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [clearLeveling(Project project)](#clearLeveling-com.aspose.tasks.Project-) | Cancella qualsiasi ritardo di livellamento che era stato precedentemente aggiunto al progetto durante il livellamento delle risorse. |
| [clearLeveling(Iterable&lt;Task&gt; tasks)](#clearLeveling-java.lang.Iterable-com.aspose.tasks.Task--) | Cancella qualsiasi ritardo di livellamento che era stato precedentemente aggiunto alle attività specificate durante il livellamento delle risorse. |
| [levelAll(Project project)](#levelAll-com.aspose.tasks.Project-) | Livella le attività per tutte le risorse del progetto utilizzando le opzioni di livellamento predefinite. |
| [levelResources(Project project, LevelingOptions options)](#levelResources-com.aspose.tasks.Project-com.aspose.tasks.LevelingOptions-) | Livella le attività per le risorse specificate utilizzando le opzioni di livellamento specificate. |
### ResourceLeveler() {#ResourceLeveler--}
```
public ResourceLeveler()
```


### clearLeveling(Project project) {#clearLeveling-com.aspose.tasks.Project-}
```
public static void clearLeveling(Project project)
```


Cancella qualsiasi ritardo di livellamento che era stato precedentemente aggiunto al progetto durante il livellamento delle risorse.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| project | [Project](../../com.aspose.tasks/project) | Progetto per cancellare il livellamento. |

### clearLeveling(Iterable&lt;Task&gt; tasks) {#clearLeveling-java.lang.Iterable-com.aspose.tasks.Task--}
```
public static void clearLeveling(Iterable<Task> tasks)
```


Cancella qualsiasi ritardo di livellamento che era stato precedentemente aggiunto alle attività specificate durante il livellamento delle risorse.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| attività | java.lang.Iterable&lt;com.aspose.tasks.Task&gt; | L'enumerabile contenente le attività per le quali il ritardo di livellamento dovrebbe essere cancellato. |

### levelAll(Project project) {#levelAll-com.aspose.tasks.Project-}
```
public static LevelingResult levelAll(Project project)
```


Livella le attività per tutte le risorse del progetto utilizzando le opzioni di livellamento predefinite.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| project | [Project](../../com.aspose.tasks/project) | Progetto per applicare il livellamento delle risorse. |

**Returns:**
[LevelingResult](../../com.aspose.tasks/levelingresult) - Object containing results of resource leveling.
### levelResources(Project project, LevelingOptions options) {#levelResources-com.aspose.tasks.Project-com.aspose.tasks.LevelingOptions-}
```
public static LevelingResult levelResources(Project project, LevelingOptions options)
```


Livella le attività per le risorse specificate utilizzando le opzioni di livellamento specificate.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| project | [Project](../../com.aspose.tasks/project) | Progetto per applicare il livellamento delle risorse. |
| options | [LevelingOptions](../../com.aspose.tasks/levelingoptions) | Opzioni che specificano come livellare le risorse. |

**Returns:**
[LevelingResult](../../com.aspose.tasks/levelingresult) - Object containing results of resource leveling.
