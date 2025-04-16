---
title: Task.MoveToSibling
second_title: Aspose.Tasks for .NET API Reference
description: Task method. Moves the current task at the same Outline Level before the specified task. If ParentProject.CalculationMode is None user should invoke Project.Recalculate after using this method It will reschedule all project tasks start/finish dates sets early/late dates and calculate the dependent fields such as slacks work and cost fields outline levels. If ParentProject.CalculationMode is Manual the method will calculate only task id outline level and outline numbers automatically. If ParentProject.CalculationMode is Automatic the method reschedules all projects tasks automatically start/finish dates sets early/late dates calculates slacks work and cost fields recalculates ids and outline levels
type: docs
weight: 1370
url: /net/aspose.tasks/task/movetosibling/
---
## MoveToSibling(Task) {#movetosibling}

Moves the current task at the same Outline Level before the specified task. If ParentProject.CalculationMode is None user should invoke Project.Recalculate() after using this method (It will reschedule all project tasks (start/finish dates, sets early/late dates) and calculate the dependent fields such as slacks, work and cost fields, outline levels). If ParentProject.CalculationMode is Manual the method will calculate only task id, outline level and outline numbers automatically. If ParentProject.CalculationMode is Automatic the method reschedules all project's tasks automatically (start/finish dates, sets early/late dates, calculates slacks, work and cost fields, recalculates ids and outline levels).

```csharp
public void MoveToSibling(Task beforeTask)
```

| Parameter | Type | Description |
| --- | --- | --- |
| beforeTask | Task | Task before which the current task will be inserted. |

## Examples

Shows how to move the task under the same parent.

```csharp
var project = new Project(DataDir + "MoveTask.mpp");

// Move tasks with id 5 before task with id 3
var task = project.RootTask.Children.GetById(5);

var targetTask = project.RootTask.Children.First(t => t.Get(Tsk.Name) == "Task4");
task.MoveToSibling(targetTask);

// OR
// Move task to the end of the collection
// task.MoveToSibling(null);
project.Save(OutDir + "MoveTaskUnderSameParent_out.mpp", SaveFileFormat.Mpp);
```

### See Also

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)

---

## MoveToSibling(int) {#movetosibling_1}

Moves the current task at the same Outline Level before a task with the specified Id. If ParentProject.CalculationMode is None user should invoke Project.Recalculate() after using this method (It will reschedule all project tasks (start/finish dates, sets early/late dates) and calculate the dependent fields such as slacks, work and cost fields, outline levels). If ParentProject.CalculationMode is Manual the method will calculate only task id, outline level and outline numbers automatically. If ParentProject.CalculationMode is Automatic the method reschedules all project's tasks automatically (start/finish dates, sets early/late dates, calculates slacks, work and cost fields, recalculates ids and outline levels).

```csharp
public void MoveToSibling(int beforeTaskId)
```

| Parameter | Type | Description |
| --- | --- | --- |
| beforeTaskId | Int32 | Id ([`Id`](../../tsk/id/)) of a task before which the current task will be inserted. |

## Examples

Shows how to move the task under the same parent using task's Id.

```csharp
var project = new Project(DataDir + "MoveTask.mpp");

// Move tasks with id 5 before task with id 3
var task = project.RootTask.Children.GetById(5);

task.MoveToSibling(3);

// OR
// Move task to the end of the collection
// task.MoveToSibling(-1);
project.Save(OutDir + "MoveTaskUnderSameParent_out.mpp", SaveFileFormat.Mpp);
```

### See Also

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


