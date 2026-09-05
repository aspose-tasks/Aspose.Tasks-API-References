---
title: "SimpleSaveOptions"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Dit is een abstracte basisklasse die de gebruiker in staat stelt basisopties op te geven bij het opslaan van een project in een bepaald formaat."
type: docs
weight: 277
url: /nl/java/com.aspose.tasks/simplesaveoptions/
---

**Inheritance:**
java.lang.Object
```
public abstract class SimpleSaveOptions
```

Dit is een abstracte basisklasse die de gebruiker in staat stelt basisopties op te geven bij het opslaan van een project in een bepaald formaat.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [SimpleSaveOptions()](#SimpleSaveOptions--) |  |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [getSaveFormat()](#getSaveFormat--) | Haalt het formaat op waarin het document wordt opgeslagen als dit opslaanopties-object wordt gebruikt. |
| [getTasksComparer()](#getTasksComparer--) | Haalt de comparer op om taken te sorteren op de Gantt-diagram en de Taakblad-diagram. |
| [getTasksFilter()](#getTasksFilter--) | Haalt de voorwaarde op die wordt gebruikt om taken te filteren die worden weergegeven op Gantt-, Taakblad- en Taakgebruik-diagrammen. |
| [setTasksComparer(Comparator&lt;Task&gt; value)](#setTasksComparer-java.util.Comparator-com.aspose.tasks.Task--) | Stelt de comparer in om taken te sorteren op de Gantt-diagram en de Taakblad-diagram. |
| [setTasksFilter(ICondition&lt;Task&gt; value)](#setTasksFilter-com.aspose.tasks.ICondition-com.aspose.tasks.Task--) | Stelt de voorwaarde in die wordt gebruikt om taken te filteren die worden weergegeven op Gantt-, Taakblad- en Taakgebruik-diagrammen. |
### SimpleSaveOptions() {#SimpleSaveOptions--}
```
public SimpleSaveOptions()
```


### getSaveFormat() {#getSaveFormat--}
```
public final int getSaveFormat()
```


Haalt het formaat op waarin het document wordt opgeslagen als dit opslaanopties-object wordt gebruikt.

**Returns:**
int - de [SaveFileFormat](../../com.aspose.tasks/savefileformat) waarin het document wordt opgeslagen.
### getTasksComparer() {#getTasksComparer--}
```
public final Comparator<Task> getTasksComparer()
```


Haalt de comparer op om taken te sorteren op de Gantt-diagram en de Taakblad-diagram.

**Returns:**
java.util.Comparator&lt;com.aspose.tasks.Task&gt; - de comparer om taken te sorteren op de Gantt-diagram en de Taakblad-diagram.
### getTasksFilter() {#getTasksFilter--}
```
public final ICondition<Task> getTasksFilter()
```


Haalt de voorwaarde op die wordt gebruikt om taken te filteren die worden weergegeven op Gantt-, Taakblad- en Taakgebruik-diagrammen.

--------------------

Als de waarde niet is opgegeven, wordt de standaardfilter gebruikt die niet-zichtbare taken verwijdert — d.w.z. onderliggende taken van samengevouwen taken.

**Returns:**
[ICondition](../../com.aspose.tasks/icondition) - the condition which is used to filter tasks rendered on Gantt, Task Sheet and Task Usage charts.
### setTasksComparer(Comparator&lt;Task&gt; value) {#setTasksComparer-java.util.Comparator-com.aspose.tasks.Task--}
```
public final void setTasksComparer(Comparator<Task> value)
```


Stelt de comparer in om taken te sorteren op de Gantt-diagram en de Taakblad-diagram.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.util.Comparator&lt;com.aspose.tasks.Task&gt; | de comparer om taken te sorteren op de Gantt-diagram en de Taakblad-diagram. |

### setTasksFilter(ICondition&lt;Task&gt; value) {#setTasksFilter-com.aspose.tasks.ICondition-com.aspose.tasks.Task--}
```
public final void setTasksFilter(ICondition<Task> value)
```


Stelt de voorwaarde in die wordt gebruikt om taken te filteren die worden weergegeven op Gantt-, Taakblad- en Taakgebruik-diagrammen.

--------------------

Als de waarde niet is opgegeven, wordt de standaardfilter gebruikt die niet-zichtbare taken verwijdert — d.w.z. onderliggende taken van samengevouwen taken.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | com.aspose.tasks.ICondition&lt;com.aspose.tasks.Task&gt; | de voorwaarde die wordt gebruikt om taken te filteren die worden weergegeven op Gantt-, Taakblad- en Taakgebruikgrafieken. |

