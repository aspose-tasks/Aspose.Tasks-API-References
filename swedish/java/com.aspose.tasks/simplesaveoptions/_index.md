---
title: "SimpleSaveOptions"
second_title: "Aspose.Tasks for Java API-referens"
description: "Detta är en abstrakt basklass som låter användaren ange grundläggande alternativ när ett projekt sparas i ett specifikt format."
type: docs
weight: 277
url: /sv/java/com.aspose.tasks/simplesaveoptions/
---

**Inheritance:**
java.lang.Object
```
public abstract class SimpleSaveOptions
```

Detta är en abstrakt basklass som låter användaren ange grundläggande alternativ när ett projekt sparas i ett specifikt format.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [SimpleSaveOptions()](#SimpleSaveOptions--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [getSaveFormat()](#getSaveFormat--) | Hämtar formatet som dokumentet kommer att sparas i om detta spara-alternativobjekt används. |
| [getTasksComparer()](#getTasksComparer--) | Hämtar jämförare för att sortera uppgifter i Gantt-diagrammet och Uppgiftsblad-diagrammet. |
| [getTasksFilter()](#getTasksFilter--) | Hämtar villkoret som används för att filtrera uppgifter som visas på Gantt-, Task Sheet- och Task Usage-diagram. |
| [setTasksComparer(Comparator&lt;Task&gt; value)](#setTasksComparer-java.util.Comparator-com.aspose.tasks.Task--) | Ställer in jämförare för att sortera uppgifter på Gantt-diagrammet och Task Sheet-diagrammet. |
| [setTasksFilter(ICondition&lt;Task&gt; value)](#setTasksFilter-com.aspose.tasks.ICondition-com.aspose.tasks.Task--) | Ställer in villkoret som används för att filtrera uppgifter som visas på Gantt-, Task Sheet- och Task Usage-diagram. |
### SimpleSaveOptions() {#SimpleSaveOptions--}
```
public SimpleSaveOptions()
```


### getSaveFormat() {#getSaveFormat--}
```
public final int getSaveFormat()
```


Hämtar formatet som dokumentet kommer att sparas i om detta spara-alternativobjekt används.

**Returns:**
int - den [SaveFileFormat](../../com.aspose.tasks/savefileformat) i vilken dokumentet kommer att sparas.
### getTasksComparer() {#getTasksComparer--}
```
public final Comparator<Task> getTasksComparer()
```


Hämtar jämförare för att sortera uppgifter i Gantt-diagrammet och Uppgiftsblad-diagrammet.

**Returns:**
java.util.Comparator&lt;com.aspose.tasks.Task&gt; - jämförare för att sortera uppgifter på Gantt-diagrammet och Task Sheet-diagrammet.
### getTasksFilter() {#getTasksFilter--}
```
public final ICondition<Task> getTasksFilter()
```


Hämtar villkoret som används för att filtrera uppgifter som visas på Gantt-, Task Sheet- och Task Usage-diagram.

--------------------

Om värdet inte anges används standardfiltret som tar bort osynliga uppgifter -- d.v.s. underordnade uppgifter till ihopklämda uppgifter.

**Returns:**
[ICondition](../../com.aspose.tasks/icondition) - the condition which is used to filter tasks rendered on Gantt, Task Sheet and Task Usage charts.
### setTasksComparer(Comparator&lt;Task&gt; value) {#setTasksComparer-java.util.Comparator-com.aspose.tasks.Task--}
```
public final void setTasksComparer(Comparator<Task> value)
```


Ställer in jämförare för att sortera uppgifter på Gantt-diagrammet och Task Sheet-diagrammet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.util.Comparator&lt;com.aspose.tasks.Task&gt; | jämförare för att sortera uppgifter på Gantt-diagrammet och Task Sheet-diagrammet. |

### setTasksFilter(ICondition&lt;Task&gt; value) {#setTasksFilter-com.aspose.tasks.ICondition-com.aspose.tasks.Task--}
```
public final void setTasksFilter(ICondition<Task> value)
```


Ställer in villkoret som används för att filtrera uppgifter som visas på Gantt-, Task Sheet- och Task Usage-diagram.

--------------------

Om värdet inte anges används standardfiltret som tar bort osynliga uppgifter -- d.v.s. underordnade uppgifter till ihopklämda uppgifter.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | com.aspose.tasks.ICondition&lt;com.aspose.tasks.Task&gt; | villkoret som används för att filtrera uppgifter som visas på Gantt-, Task Sheet- och Task Usage-diagram. |

