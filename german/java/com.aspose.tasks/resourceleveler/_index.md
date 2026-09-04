---
title: "ResourceLeveler"
second_title: "Aspose.Tasks for Java API Reference"
description: "Enthält Methoden zur Ressourcenlevelung."
type: docs
weight: 253
url: /de/java/com.aspose.tasks/resourceleveler/
---

**Inheritance:**
java.lang.Object
```
public class ResourceLeveler
```

Enthält Methoden zur Ressourcenlevelung.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [ResourceLeveler()](#ResourceLeveler--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [clearLeveling(Project project)](#clearLeveling-com.aspose.tasks.Project-) | Löscht jede Leveling-Verzögerung, die dem Projekt während der Ressourcen-Leveling hinzugefügt wurde. |
| [clearLeveling(Iterable&lt;Task&gt; tasks)](#clearLeveling-java.lang.Iterable-com.aspose.tasks.Task--) | Löscht jede Leveling-Verzögerung, die den angegebenen Aufgaben während des Ressourcen-Levelings hinzugefügt wurde. |
| [levelAll(Project project)](#levelAll-com.aspose.tasks.Project-) | Levelt Aufgaben für alle Ressourcen des Projekts mit den Standard-Leveling-Optionen. |
| [levelResources(Project project, LevelingOptions options)](#levelResources-com.aspose.tasks.Project-com.aspose.tasks.LevelingOptions-) | Levelt Aufgaben für die angegebenen Ressourcen mit den angegebenen Leveling-Optionen. |
### ResourceLeveler() {#ResourceLeveler--}
```
public ResourceLeveler()
```


### clearLeveling(Project project) {#clearLeveling-com.aspose.tasks.Project-}
```
public static void clearLeveling(Project project)
```


Löscht jede Leveling-Verzögerung, die dem Projekt während der Ressourcen-Leveling hinzugefügt wurde.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| project | [Project](../../com.aspose.tasks/project) | Projekt zum Löschen des Levelings. |

### clearLeveling(Iterable&lt;Task&gt; tasks) {#clearLeveling-java.lang.Iterable-com.aspose.tasks.Task--}
```
public static void clearLeveling(Iterable<Task> tasks)
```


Löscht jede Leveling-Verzögerung, die den angegebenen Aufgaben während des Ressourcen-Levelings hinzugefügt wurde.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Aufgaben | java.lang.Iterable&lt;com.aspose.tasks.Task&gt; | Die Aufzählung, die Aufgaben enthält, für die die Leveling-Verzögerung gelöscht werden soll. |

### levelAll(Project project) {#levelAll-com.aspose.tasks.Project-}
```
public static LevelingResult levelAll(Project project)
```


Levelt Aufgaben für alle Ressourcen des Projekts mit den Standard-Leveling-Optionen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| project | [Project](../../com.aspose.tasks/project) | Projekt zur Anwendung des Ressourcen-Levelings. |

**Returns:**
[LevelingResult](../../com.aspose.tasks/levelingresult) - Object containing results of resource leveling.
### levelResources(Project project, LevelingOptions options) {#levelResources-com.aspose.tasks.Project-com.aspose.tasks.LevelingOptions-}
```
public static LevelingResult levelResources(Project project, LevelingOptions options)
```


Levelt Aufgaben für die angegebenen Ressourcen mit den angegebenen Leveling-Optionen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| project | [Project](../../com.aspose.tasks/project) | Projekt zur Anwendung des Ressourcen-Levelings. |
| options | [LevelingOptions](../../com.aspose.tasks/levelingoptions) | Optionen, die festlegen, wie Ressourcen zu leveln sind. |

**Returns:**
[LevelingResult](../../com.aspose.tasks/levelingresult) - Object containing results of resource leveling.
