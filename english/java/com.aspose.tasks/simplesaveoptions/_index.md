---
title: SimpleSaveOptions
second_title: Aspose.Tasks for Java API Reference
description: This is an abstract base class that allow the user to specify basic options when saving a project into a particular format.
type: docs
weight: 276
url: /java/com.aspose.tasks/simplesaveoptions/
---

**Inheritance:**
java.lang.Object
```
public abstract class SimpleSaveOptions
```

This is an abstract base class that allow the user to specify basic options when saving a project into a particular format.
## Constructors

| Constructor | Description |
| --- | --- |
| [SimpleSaveOptions()](#SimpleSaveOptions--) |  |
## Methods

| Method | Description |
| --- | --- |
| [getSaveFormat()](#getSaveFormat--) | Gets the format in which the document will be saved if this save options object is used. |
| [getTasksComparer()](#getTasksComparer--) | Gets the comparer to sort tasks on Gantt chart and Task Sheet chart. |
| [getTasksFilter()](#getTasksFilter--) | Gets the condition which is used to filter tasks rendered on Gantt, Task Sheet and Task Usage charts. |
| [setTasksComparer(Comparator&lt;Task&gt; value)](#setTasksComparer-java.util.Comparator-com.aspose.tasks.Task--) | Sets the comparer to sort tasks on Gantt chart and Task Sheet chart. |
| [setTasksFilter(ICondition&lt;Task&gt; value)](#setTasksFilter-com.aspose.tasks.ICondition-com.aspose.tasks.Task--) | Sets the condition which is used to filter tasks rendered on Gantt, Task Sheet and Task Usage charts. |
### SimpleSaveOptions() {#SimpleSaveOptions--}
```
public SimpleSaveOptions()
```


### getSaveFormat() {#getSaveFormat--}
```
public final int getSaveFormat()
```


Gets the format in which the document will be saved if this save options object is used.

**Returns:**
int - the [SaveFileFormat](../../com.aspose.tasks/savefileformat) in which the document will be saved.
### getTasksComparer() {#getTasksComparer--}
```
public final Comparator<Task> getTasksComparer()
```


Gets the comparer to sort tasks on Gantt chart and Task Sheet chart.

**Returns:**
java.util.Comparator&lt;com.aspose.tasks.Task&gt; - the comparer to sort tasks on Gantt chart and Task Sheet chart.
### getTasksFilter() {#getTasksFilter--}
```
public final ICondition<Task> getTasksFilter()
```


Gets the condition which is used to filter tasks rendered on Gantt, Task Sheet and Task Usage charts.

--------------------

If value is not specified the default filter is used which removes non-visible tasks -- i.e. descendant tasks of collapsed tasks.

**Returns:**
[ICondition](../../com.aspose.tasks/icondition) - the condition which is used to filter tasks rendered on Gantt, Task Sheet and Task Usage charts.
### setTasksComparer(Comparator&lt;Task&gt; value) {#setTasksComparer-java.util.Comparator-com.aspose.tasks.Task--}
```
public final void setTasksComparer(Comparator<Task> value)
```


Sets the comparer to sort tasks on Gantt chart and Task Sheet chart.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Comparator&lt;com.aspose.tasks.Task&gt; | the comparer to sort tasks on Gantt chart and Task Sheet chart. |

### setTasksFilter(ICondition&lt;Task&gt; value) {#setTasksFilter-com.aspose.tasks.ICondition-com.aspose.tasks.Task--}
```
public final void setTasksFilter(ICondition<Task> value)
```


Sets the condition which is used to filter tasks rendered on Gantt, Task Sheet and Task Usage charts.

--------------------

If value is not specified the default filter is used which removes non-visible tasks -- i.e. descendant tasks of collapsed tasks.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | com.aspose.tasks.ICondition&lt;com.aspose.tasks.Task&gt; | the condition which is used to filter tasks rendered on Gantt, Task Sheet and Task Usage charts. |

