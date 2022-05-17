---
title: Task
second_title: Aspose.Tasks for .NET API Reference
description: 
type: docs
weight: 2060
url: /net/aspose.tasks/task/
---
## Task class

Represents a task in a project.

```csharp
public class Task : IEquatable<Task>
```

## Properties

| Name | Description |
| --- | --- |
| [Assignments](assignments) { get; } | Gets a collection of resource assignments for this object. |
| [Baselines](baselines) { get; set; } | Gets or sets the collection of baseline values of the task. |
| [Children](children) { get; } | Gets a child task collection of this object. TaskCollection object which represents children tasks. |
| [ExtendedAttributes](extendedattributes) { get; } | Gets ExtendedAttributeCollection object containing the values of an extended attribute. |
| [OutlineCodes](outlinecodes) { get; set; } | Gets or sets [`OutlineCodeCollection`](../outlinecodecollection) object. |
| [ParentProject](parentproject) { get; } | Gets the parent project of a task. |
| [ParentTask](parenttask) { get; } | Gets the parent task of a task. |
| [Predecessors](predecessors) { get; } | Gets a [`TaskCollection`](../taskcollection) object which contains all predecessors of this Task object. |
| [RecurringInfo](recurringinfo) { get; } | Gets the instance of [`RecurringTaskInfo`](../recurringtaskinfo) class for the task which is a recurring task; if the task is not a recurring one then returns null; The info for the instance of [`RecurringTaskInfo`](../recurringtaskinfo) is present in mpp file format only. |
| [SplitParts](splitparts) { get; } | Gets a SplitPart collection that represents the portions of a task. |
| [Successors](successors) { get; } | Gets a [`TaskCollection`](../taskcollection) object which contains all successors of this Task object. |
| [TimephasedData](timephaseddata) { get; set; } | Gets or sets a TimephasedDataCollection object of this task. The time phased data block associated with a task. |

## Methods

| Name | Description |
| --- | --- |
| [Clone](clone)() | Creates full copy of a task without subtasks. |
| [Delete](delete)() | Deletes a task from parent project tasks collection and all its assignments. |
| override [Equals](equals)(object) | Returns a value indicating whether this instance is equal to a specified object. |
| [Equals](equals)(Task) | Returns a value indicating whether this instance is equal to a specified task. |
| [Get&lt;T&gt;](get)(Key&lt;T, TaskKey&gt;) | Returns the value to which the property is mapped in this container. |
| override [GetHashCode](gethashcode)() | Returns a hash code value for this Task. |
| [GetTimephasedData](gettimephaseddata)(DateTime, DateTime) | Returns [`TimephasedDataCollection`](../timephaseddatacollection) object with [`TimephasedData`](./timephaseddata) values within given start and end dates. |
| [GetTimephasedData](gettimephaseddata)(DateTime, DateTime, TimephasedDataType) | Returns [`TimephasedDataCollection`](../timephaseddatacollection) object with [`TimephasedData`](./timephaseddata) values within given start and end dates of specified time-phased data type. |
| [MoveToSibling](movetosibling)(int) | Moves the current task at the same Outline Level before a task with the specified Id. If ParentProject.CalculationMode is None user should invoke Project.Recalculate() after using this method (It will reschedule all project tasks (start/finish dates, sets early/late dates) and calculate the dependent fields such as slacks, work and cost fields, outline levels). If ParentProject.CalculationMode is Manual the method will calculate only task id, outline level and outline numbers automatically. If ParentProject.CalculationMode is Automatic the method reschedules all project's tasks automatically (start/finish dates, sets early/late dates, calculates slacks, work and cost fields, recalculates ids and outline levels). |
| [MoveToSibling](movetosibling)(Task) | Moves the current task at the same Outline Level before the specified task. If ParentProject.CalculationMode is None user should invoke Project.Recalculate() after using this method (It will reschedule all project tasks (start/finish dates, sets early/late dates) and calculate the dependent fields such as slacks, work and cost fields, outline levels). If ParentProject.CalculationMode is Manual the method will calculate only task id, outline level and outline numbers automatically. If ParentProject.CalculationMode is Automatic the method reschedules all project's tasks automatically (start/finish dates, sets early/late dates, calculates slacks, work and cost fields, recalculates ids and outline levels). |
| [OutlineIndent](outlineindent)() | Indents a task in the outline. |
| [OutlineOutdent](outlineoutdent)() | Promotes a task in the outline. |
| [SelectAllChildTasks](selectallchildtasks)() | Recursively collects all child tasks of this task. |
| [Set&lt;T&gt;](set)(Key&lt;T, TaskKey&gt;, T) | Maps the specified property to the specified value in this container. |
| override [ToString](tostring)() | Returns short string representation of a task. The exact details of the representation are unspecified and subject to change. |

### Remarks

The **Task** is representing a one atomic chuck of work.

One can use **Task** to plan a project by creating tasks and assign appropriate resources onto them. Tasks in a project are organized as a rooted hierarchical tree structure, with a root task and subtrees of children tasks.

To build a tree of tasks one can use a specialized collection [`TaskCollection`](../taskcollection) by accessing [`RootTask`](../project/roottask) property e.g.:

```csharp
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
project.Save("Filled project.xml", SaveFileFormat.MPP);
```

### See Also

* namespace [Aspose.Tasks](../../aspose.tasks)
* assembly [Aspose.Tasks](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
