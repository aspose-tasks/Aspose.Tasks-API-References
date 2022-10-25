---
title: Task
second_title: Aspose.Tasks for Java API Reference
description: Represents a task in a project.
type: docs
weight: 263
url: /java/com.aspose.tasks/task/
---

**Inheritance:**
java.lang.Object, com.aspose.tasks.IContainer

**All Implemented Interfaces:**
com.aspose.ms.System.IEquatable, com.aspose.tasks.IExtendedAttributeParent, java.lang.Cloneable
```
public class Task extends IContainer<Integer> implements System.IEquatable<Task>, IExtendedAttributeParent, Cloneable
```

Represents a task in a project.

--------------------

The **Task** is representing a one atomic chuck of work.

One can use **Task** to plan a project by creating tasks and assign appropriate resources onto them. Tasks in a project are organized as a rooted hierarchical tree structure, with a root task and subtrees of children tasks.

To build a tree of tasks one can use a specialized collection [TaskCollection](../../com.aspose.tasks/taskcollection) by accessing  Project.RootTask ([Project.getRootTask](../../com.aspose.tasks/project\#getRootTask)/[Project.setRootTask(Task)](../../com.aspose.tasks/project\#setRootTask-Task-)) property e.g.:

```

  Project project = new Project();
  // add new tasks
  Task task1 = project.RootTask.Children.Add(); // a parent task with empty name is added
  Task childTask1 = task1.Children.Add("Child 1");
  childTask1.Set(Tsk.Start, new DateTime(2020, 2, 12, 8, 0, 0))
  childTask1.Set(Tsk.Duration, project.GetDuration(8, TimeUnitType.Hour));
  childTask1.Set(Tsk.Finish, new DateTime(2020, 2, 12, 17, 0, 0));
  Task childTask3 = task1.Children.Add("Child 3");
  childTask3.Set(Tsk.Start, new DateTime(2020, 2, 13, 8, 0, 0))
  childTask3.Set(Tsk.Duration, project.GetDuration(8, TimeUnitType.Hour));
  childTask3.Set(Tsk.Finish, new DateTime(2020, 2, 13, 17, 0, 0));
  Task childTask2 = task1.Children.Add("Child 2", 2); // inserts a task before the childTask3
  childTask2.Set(Tsk.Start, new DateTime(2020, 2, 14, 8, 0, 0))
  childTask2.Set(Tsk.Duration, project.GetDuration(8, TimeUnitType.Hour));
  childTask2.Set(Tsk.Finish, new DateTime(2020, 2, 14, 17, 0, 0));

  // save project in the one of available formats
  project.Save("Filled project.xml", SaveFileFormat.Mpp);
  
```
## Methods

| Method | Description |
| --- | --- |
| [deepClone()](#deepClone--) | Creates full copy of a task without subtasks. |
| [delete()](#delete--) | Deletes a task from parent project tasks collection and all its assignments. |
| [equals(Task other)](#equals-com.aspose.tasks.Task-) | Returns a value indicating whether this instance is equal to a specified task. |
| [equals(Object obj)](#equals-java.lang.Object-) | Returns a value indicating whether this instance is equal to a specified object. |
| [&lt;T&gt;get(Key&lt;T,Integer&gt; key)](#-T-get-com.aspose.tasks.Key-T-java.lang.Integer--) | Returns the value to which the property is mapped in this container. |
| [getAssignments()](#getAssignments--) | Gets a collection of resource assignments for this object. |
| [getBaselines()](#getBaselines--) | Gets the collection of baseline values of the task. |
| [setBaselines(TaskBaselineCollection value)](#setBaselines-com.aspose.tasks.TaskBaselineCollection-) | Sets the collection of baseline values of the task. |
| [getChildren()](#getChildren--) | Gets a child task collection of this object. |
| [getExtendedAttributes()](#getExtendedAttributes--) | Gets ExtendedAttributeCollection object containing the values of an extended attribute. |
| [getItems()](#getItems--) | \{@inheritDoc\} |
| [getOutlineCodes()](#getOutlineCodes--) | Gets [OutlineCodeCollection](../../com.aspose.tasks/outlinecodecollection) object. |
| [setOutlineCodes(OutlineCodeCollection value)](#setOutlineCodes-com.aspose.tasks.OutlineCodeCollection-) | Sets [OutlineCodeCollection](../../com.aspose.tasks/outlinecodecollection) object. |
| [getParentProject()](#getParentProject--) | Gets the parent project of a task. |
| [getParentTask()](#getParentTask--) | Gets the parent task of a task. |
| [getPredecessors()](#getPredecessors--) | Gets a [TaskCollection](../../com.aspose.tasks/taskcollection) object which contains all predecessors of this Task object. |
| [getRecurringInfo()](#getRecurringInfo--) | Gets the instance of [RecurringTaskInfo](../../com.aspose.tasks/recurringtaskinfo) class for the task which is a recurring task; if the task is not a recurring one then returns null; |
| [getSplitParts()](#getSplitParts--) | Gets a SplitPart collection that represents the portions of a task. |
| [getSuccessors()](#getSuccessors--) | Gets a [TaskCollection](../../com.aspose.tasks/taskcollection) object which contains all successors of this Task object. |
| [getTimephasedData()](#getTimephasedData--) | Gets a TimephasedDataCollection object of this task. |
| [setTimephasedData(TimephasedDataCollection value)](#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-) | Sets a TimephasedDataCollection object of this task. |
| [getTimephasedData(Date start, Date end, int timephasedType)](#getTimephasedData-java.util.Date-java.util.Date-int-) | Returns [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) object with  TimephasedData ([getTimephasedData()](../../com.aspose.tasks/task\#getTimephasedData--)/[setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/task\#setTimephasedData-TimephasedDataCollection-)) values within given start and end dates of specified time-phased data type. |
| [getTimephasedData(Date start, Date end)](#getTimephasedData-java.util.Date-java.util.Date-) | Returns [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) object with  TimephasedData ([getTimephasedData()](../../com.aspose.tasks/task\#getTimephasedData--)/[setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/task\#setTimephasedData-TimephasedDataCollection-)) values within given start and end dates. |
| [hasChildren()](#hasChildren--) | Gets a value indicating that this task has children. |
| [hashCode()](#hashCode--) | Returns a hash code value for this Task. |
| [moveToSibling(Task beforeTask)](#moveToSibling-com.aspose.tasks.Task-) | Moves the current task at the same Outline Level before the specified task. |
| [moveToSibling(int beforeTaskId)](#moveToSibling-int-) | Moves the current task at the same Outline Level before a task with the specified Id. |
| [outlineIndent()](#outlineIndent--) | Indents a task in the outline. |
| [outlineOutdent()](#outlineOutdent--) | Promotes a task in the outline. |
| [selectAllChildTasks()](#selectAllChildTasks--) | Recursively collects all child tasks of this task. |
| [&lt;T&gt;set(Key&lt;T,Integer&gt; key, T val)](#-T-set-com.aspose.tasks.Key-T-java.lang.Integer--T-) | Maps the specified property to the specified value in this container. |
| [set(Key&lt;Date,Integer&gt; key, Date val)](#set-com.aspose.tasks.Key-java.util.Date-java.lang.Integer--java.util.Date-) | Maps the specified property to the specified value in this container. |
| [toString()](#toString--) | Returns short string representation of a task. |
### deepClone() {#deepClone--}
```
public final Object deepClone()
```


Creates full copy of a task without subtasks.

**Returns:**
java.lang.Object - Created copy of a task.
### delete() {#delete--}
```
public final void delete()
```


Deletes a task from parent project tasks collection and all its assignments.

### equals(Task other) {#equals-com.aspose.tasks.Task-}
```
public final boolean equals(Task other)
```


Returns a value indicating whether this instance is equal to a specified task.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| other | [Task](../../com.aspose.tasks/task) | The specified task to compare with this instance. |

**Returns:**
boolean - returns true if the specified task and this instance have equal unique ids.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Returns a value indicating whether this instance is equal to a specified object.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | java.lang.Object | The specified object to compare with this instance. |

**Returns:**
boolean - returns true if the specified task and this instance have equal unique ids.
### &lt;T&gt;get(Key&lt;T,Integer&gt; key) {#-T-get-com.aspose.tasks.Key-T-java.lang.Integer--}
```
public final T <T>get(Key<T,Integer> key)
```


Returns the value to which the property is mapped in this container.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;T,java.lang.Integer&gt; | the specified property key. [Tsk](../../com.aspose.tasks/tsk) for getting the property key.

 T : the type of the mapped value. |

**Returns:**
T - the value to which the property is mapped in this container.
### getAssignments() {#getAssignments--}
```
public final ResourceAssignmentCollection getAssignments()
```


Gets a collection of resource assignments for this object.

**Returns:**
[ResourceAssignmentCollection](../../com.aspose.tasks/resourceassignmentcollection) - a collection of resource assignments for this object.
### getBaselines() {#getBaselines--}
```
public final TaskBaselineCollection getBaselines()
```


Gets the collection of baseline values of the task.

**Returns:**
[TaskBaselineCollection](../../com.aspose.tasks/taskbaselinecollection) - the collection of baseline values of the task.
### setBaselines(TaskBaselineCollection value) {#setBaselines-com.aspose.tasks.TaskBaselineCollection-}
```
public final void setBaselines(TaskBaselineCollection value)
```


Sets the collection of baseline values of the task.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TaskBaselineCollection](../../com.aspose.tasks/taskbaselinecollection) | the collection of baseline values of the task. |

### getChildren() {#getChildren--}
```
public final TaskCollection getChildren()
```


Gets a child task collection of this object. TaskCollection object which represents children tasks.

**Returns:**
[TaskCollection](../../com.aspose.tasks/taskcollection) - a child task collection of this object.
### getExtendedAttributes() {#getExtendedAttributes--}
```
public final ExtendedAttributeCollection getExtendedAttributes()
```


Gets ExtendedAttributeCollection object containing the values of an extended attribute.

--------------------

Two pieces of data are necessary - a pointer back to the extended attribute table which is specified either by the unique ID or the Field ID, and the value which is specified either with the value, or a pointer back to the value list.

**Returns:**
[ExtendedAttributeCollection](../../com.aspose.tasks/extendedattributecollection) - ExtendedAttributeCollection object containing the values of an extended attribute.
### getItems() {#getItems--}
```
public final System.Collections.Generic.IGenericEnumerable<IExtendedAttributeParent> getItems()
```


Reserved for internal usage.

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerable&lt;com.aspose.tasks.IExtendedAttributeParent&gt; - \{@inheritDoc\}
### getOutlineCodes() {#getOutlineCodes--}
```
public final OutlineCodeCollection getOutlineCodes()
```


Gets [OutlineCodeCollection](../../com.aspose.tasks/outlinecodecollection) object.

--------------------

Two pieces of data are necessary - a pointer to the outline code table that is specified by the FieldID, and the value that is specified either by the ValueID or ValueGUID pointer to the value list.

**Returns:**
[OutlineCodeCollection](../../com.aspose.tasks/outlinecodecollection) - [OutlineCodeCollection](../../com.aspose.tasks/outlinecodecollection) object.
### setOutlineCodes(OutlineCodeCollection value) {#setOutlineCodes-com.aspose.tasks.OutlineCodeCollection-}
```
public final void setOutlineCodes(OutlineCodeCollection value)
```


Sets [OutlineCodeCollection](../../com.aspose.tasks/outlinecodecollection) object.

--------------------

Two pieces of data are necessary - a pointer to the outline code table that is specified by the FieldID, and the value that is specified either by the ValueID or ValueGUID pointer to the value list.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [OutlineCodeCollection](../../com.aspose.tasks/outlinecodecollection) | [OutlineCodeCollection](../../com.aspose.tasks/outlinecodecollection) object. |

### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


Gets the parent project of a task.

--------------------

Call Project.UpdateReferences to update these properties.

**Returns:**
[Project](../../com.aspose.tasks/project) - the parent project of a task.
### getParentTask() {#getParentTask--}
```
public final Task getParentTask()
```


Gets the parent task of a task.

**Returns:**
[Task](../../com.aspose.tasks/task) - the parent task of a task.
### getPredecessors() {#getPredecessors--}
```
public final TaskCollection getPredecessors()
```


Gets a [TaskCollection](../../com.aspose.tasks/taskcollection) object which contains all predecessors of this Task object.

**Returns:**
[TaskCollection](../../com.aspose.tasks/taskcollection) - Read-only instance of [TaskCollection](../../com.aspose.tasks/taskcollection) class.
### getRecurringInfo() {#getRecurringInfo--}
```
public final RecurringTaskInfo getRecurringInfo()
```


Gets the instance of [RecurringTaskInfo](../../com.aspose.tasks/recurringtaskinfo) class for the task which is a recurring task; if the task is not a recurring one then returns null;

--------------------

The info for the instance of [RecurringTaskInfo](../../com.aspose.tasks/recurringtaskinfo) is present in mpp file format only.

**Returns:**
[RecurringTaskInfo](../../com.aspose.tasks/recurringtaskinfo) - the instance of [RecurringTaskInfo](../../com.aspose.tasks/recurringtaskinfo) class for the task which is a recurring task; if the task is not a recurring one then returns null;
### getSplitParts() {#getSplitParts--}
```
public final SplitPartCollection getSplitParts()
```


Gets a SplitPart collection that represents the portions of a task.

**Returns:**
[SplitPartCollection](../../com.aspose.tasks/splitpartcollection) - a SplitPart collection that represents the portions of a task.
### getSuccessors() {#getSuccessors--}
```
public final TaskCollection getSuccessors()
```


Gets a [TaskCollection](../../com.aspose.tasks/taskcollection) object which contains all successors of this Task object.

**Returns:**
[TaskCollection](../../com.aspose.tasks/taskcollection) - Read-only instance of [TaskCollection](../../com.aspose.tasks/taskcollection) class.
### getTimephasedData() {#getTimephasedData--}
```
public final TimephasedDataCollection getTimephasedData()
```


Gets a TimephasedDataCollection object of this task. The time phased data block associated with a task.

--------------------

Reading supported for XML format only.

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - a TimephasedDataCollection object of this task.
### setTimephasedData(TimephasedDataCollection value) {#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-}
```
public final void setTimephasedData(TimephasedDataCollection value)
```


Sets a TimephasedDataCollection object of this task. The time phased data block associated with a task.

--------------------

Reading supported for XML format only.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) | a TimephasedDataCollection object of this task. |

### getTimephasedData(Date start, Date end, int timephasedType) {#getTimephasedData-java.util.Date-java.util.Date-int-}
```
public final TimephasedDataCollection getTimephasedData(Date start, Date end, int timephasedType)
```


Returns [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) object with  TimephasedData ([getTimephasedData()](../../com.aspose.tasks/task\#getTimephasedData--)/[setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/task\#setTimephasedData-TimephasedDataCollection-)) values within given start and end dates of specified time-phased data type.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| start | java.util.Date | The start date for the time phased data. |
| end | java.util.Date | The end date for the time phased data. |
| timephasedType | int | The type of time phased data ([TimephasedDataType](../../com.aspose.tasks/timephaseddatatype)). |

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - A [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) object with  TimephasedData ([getTimephasedData()](../../com.aspose.tasks/task\#getTimephasedData--)/\#setTimephasedData(TimephasedDataCollection).setTimephasedData(TimephasedDataCollection)) values within given start and end dates of specified timephased data type.
### getTimephasedData(Date start, Date end) {#getTimephasedData-java.util.Date-java.util.Date-}
```
public final TimephasedDataCollection getTimephasedData(Date start, Date end)
```


Returns [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) object with  TimephasedData ([getTimephasedData()](../../com.aspose.tasks/task\#getTimephasedData--)/[setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/task\#setTimephasedData-TimephasedDataCollection-)) values within given start and end dates.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| start | java.util.Date | The start date for the time phased data. |
| end | java.util.Date | The end date for the time phased data. |

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - List of [TimephasedData](../../com.aspose.tasks/timephaseddata) to be filled in.
### hasChildren() {#hasChildren--}
```
public final boolean hasChildren()
```


Gets a value indicating that this task has children.

**Returns:**
boolean - a value indicating that this task has children.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Returns a hash code value for this Task.

**Returns:**
int - returns a hash code value for this object.
### moveToSibling(Task beforeTask) {#moveToSibling-com.aspose.tasks.Task-}
```
public final void moveToSibling(Task beforeTask)
```


Moves the current task at the same Outline Level before the specified task. If ParentProject.CalculationMode is None user should invoke Project.Recalculate() after using this method (It will reschedule all project tasks (start/finish dates, sets early/late dates) and calculate the dependent fields such as slacks, work and cost fields, outline levels). If ParentProject.CalculationMode is Manual the method will calculate only task id, outline level and outline numbers automatically. If ParentProject.CalculationMode is Automatic the method reschedules all project's tasks automatically (start/finish dates, sets early/late dates, calculates slacks, work and cost fields, recalculates ids and outline levels).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| beforeTask | [Task](../../com.aspose.tasks/task) | Task before which the current task will be inserted. |

### moveToSibling(int beforeTaskId) {#moveToSibling-int-}
```
public final void moveToSibling(int beforeTaskId)
```


Moves the current task at the same Outline Level before a task with the specified Id. If ParentProject.CalculationMode is None user should invoke Project.Recalculate() after using this method (It will reschedule all project tasks (start/finish dates, sets early/late dates) and calculate the dependent fields such as slacks, work and cost fields, outline levels). If ParentProject.CalculationMode is Manual the method will calculate only task id, outline level and outline numbers automatically. If ParentProject.CalculationMode is Automatic the method reschedules all project's tasks automatically (start/finish dates, sets early/late dates, calculates slacks, work and cost fields, recalculates ids and outline levels).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| beforeTaskId | int | Id ([Tsk.ID](../../com.aspose.tasks/tsk\#ID)) of a task before which the current task will be inserted. |

### outlineIndent() {#outlineIndent--}
```
public final void outlineIndent()
```


Indents a task in the outline.

### outlineOutdent() {#outlineOutdent--}
```
public final void outlineOutdent()
```


Promotes a task in the outline.

### selectAllChildTasks() {#selectAllChildTasks--}
```
public final Iterable<Task> selectAllChildTasks()
```


Recursively collects all child tasks of this task.

**Returns:**
java.lang.Iterable&lt;com.aspose.tasks.Task&gt; - A list of child tasks of this task.
### &lt;T&gt;set(Key&lt;T,Integer&gt; key, T val) {#-T-set-com.aspose.tasks.Key-T-java.lang.Integer--T-}
```
public final void <T>set(Key<T,Integer> key, T val)
```


Maps the specified property to the specified value in this container.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;T,java.lang.Integer&gt; | the specified property key. [Tsk](../../com.aspose.tasks/tsk) for getting the property key. |
| val | T | the value.

 T : the type of the mapped value. |

### set(Key&lt;Date,Integer&gt; key, Date val) {#set-com.aspose.tasks.Key-java.util.Date-java.lang.Integer--java.util.Date-}
```
public final void set(Key<Date,Integer> key, Date val)
```


Maps the specified property to the specified value in this container.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;java.util.Date,java.lang.Integer&gt; | the specified property key. [Tsk](../../com.aspose.tasks/tsk) for getting the property key. |
| val | java.util.Date | the value. |

### toString() {#toString--}
```
public String toString()
```


Returns short string representation of a task. The exact details of the representation are unspecified and subject to change.

**Returns:**
java.lang.String - short string which represents task object.
