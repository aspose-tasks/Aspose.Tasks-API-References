---
title: "SimpleSaveOptions"
second_title: "Aspose.Tasks for Java API Reference"
description: "Dies ist eine abstrakte Basisklasse, die dem Benutzer ermöglicht, grundlegende Optionen beim Speichern eines Projekts in ein bestimmtes Format anzugeben."
type: docs
weight: 277
url: /de/java/com.aspose.tasks/simplesaveoptions/
---

**Inheritance:**
java.lang.Object
```
public abstract class SimpleSaveOptions
```

Dies ist eine abstrakte Basisklasse, die dem Benutzer ermöglicht, grundlegende Optionen beim Speichern eines Projekts in ein bestimmtes Format anzugeben.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [SimpleSaveOptions()](#SimpleSaveOptions--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getSaveFormat()](#getSaveFormat--) | Ermittelt das Format, in dem das Dokument gespeichert wird, wenn dieses Speichereinstellungsobjekt verwendet wird. |
| [getTasksComparer()](#getTasksComparer--) | Ermittelt das Vergleichsobjekt zum Sortieren von Aufgaben im Gantt-Diagramm und im Aufgabenblatt-Diagramm. |
| [getTasksFilter()](#getTasksFilter--) | Ermittelt die Bedingung, die zum Filtern von Aufgaben verwendet wird, die im Gantt-, Aufgabenblatt- und Aufgabenverwendungsdiagramm dargestellt werden. |
| [setTasksComparer(Comparator&lt;Task&gt; value)](#setTasksComparer-java.util.Comparator-com.aspose.tasks.Task--) | Legt das Vergleichsobjekt zum Sortieren von Aufgaben im Gantt-Diagramm und im Aufgabenblatt-Diagramm fest. |
| [setTasksFilter(ICondition&lt;Task&gt; value)](#setTasksFilter-com.aspose.tasks.ICondition-com.aspose.tasks.Task--) | Legt die Bedingung fest, die zum Filtern von Aufgaben verwendet wird, die im Gantt-, Aufgabenblatt- und Aufgabenverwendungsdiagramm dargestellt werden. |
### SimpleSaveOptions() {#SimpleSaveOptions--}
```
public SimpleSaveOptions()
```


### getSaveFormat() {#getSaveFormat--}
```
public final int getSaveFormat()
```


Ermittelt das Format, in dem das Dokument gespeichert wird, wenn dieses Speichereinstellungsobjekt verwendet wird.

**Returns:**
int - das [SaveFileFormat](../../com.aspose.tasks/savefileformat), in dem das Dokument gespeichert wird.
### getTasksComparer() {#getTasksComparer--}
```
public final Comparator<Task> getTasksComparer()
```


Ermittelt das Vergleichsobjekt zum Sortieren von Aufgaben im Gantt-Diagramm und im Aufgabenblatt-Diagramm.

**Returns:**
java.util.Comparator&lt;com.aspose.tasks.Task&gt; - das Vergleichsobjekt zum Sortieren von Aufgaben im Gantt-Diagramm und im Aufgabenblatt-Diagramm.
### getTasksFilter() {#getTasksFilter--}
```
public final ICondition<Task> getTasksFilter()
```


Ermittelt die Bedingung, die zum Filtern von Aufgaben verwendet wird, die im Gantt-, Aufgabenblatt- und Aufgabenverwendungsdiagramm dargestellt werden.

--------------------

Wenn kein Wert angegeben ist, wird der Standardfilter verwendet, der nicht sichtbare Aufgaben entfernt – d. h. Nachfolgeraufgaben von zusammengeklappten Aufgaben.

**Returns:**
[ICondition](../../com.aspose.tasks/icondition) - the condition which is used to filter tasks rendered on Gantt, Task Sheet and Task Usage charts.
### setTasksComparer(Comparator&lt;Task&gt; value) {#setTasksComparer-java.util.Comparator-com.aspose.tasks.Task--}
```
public final void setTasksComparer(Comparator<Task> value)
```


Legt das Vergleichsobjekt zum Sortieren von Aufgaben im Gantt-Diagramm und im Aufgabenblatt-Diagramm fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.util.Comparator&lt;com.aspose.tasks.Task&gt; | das Vergleichsobjekt zum Sortieren von Aufgaben im Gantt-Diagramm und im Aufgabenblatt-Diagramm. |

### setTasksFilter(ICondition&lt;Task&gt; value) {#setTasksFilter-com.aspose.tasks.ICondition-com.aspose.tasks.Task--}
```
public final void setTasksFilter(ICondition<Task> value)
```


Legt die Bedingung fest, die zum Filtern von Aufgaben verwendet wird, die im Gantt-, Aufgabenblatt- und Aufgabenverwendungsdiagramm dargestellt werden.

--------------------

Wenn kein Wert angegeben ist, wird der Standardfilter verwendet, der nicht sichtbare Aufgaben entfernt – d. h. Nachfolgeraufgaben von zusammengeklappten Aufgaben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | com.aspose.tasks.ICondition&lt;com.aspose.tasks.Task&gt; | die Bedingung, die zum Filtern von Aufgaben verwendet wird, die im Gantt-, Aufgabenblatt- und Aufgabenverwendungsdiagramm dargestellt werden. |

