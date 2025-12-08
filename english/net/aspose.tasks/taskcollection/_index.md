---
title: Class TaskCollection
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.TaskCollection class. Represents a collection of Task objects
type: docs
weight: 2350
url: /net/aspose.tasks/taskcollection/
---
## TaskCollection class

Represents a collection of [`Task`](../task/) objects.

```csharp
public class TaskCollection : IList<Task>
```

## Properties

| Name | Description |
| --- | --- |
| [Count](../../aspose.tasks/taskcollection/count/) { get; } | Gets the number of objects contained in the TaskCollection. |
| [IsReadOnly](../../aspose.tasks/taskcollection/isreadonly/) { get; } | Gets a value indicating whether this collection is read only. |
| [Item](../../aspose.tasks/taskcollection/item/) { get; set; } | Returns the element at the specified index. |
| [ParentProject](../../aspose.tasks/taskcollection/parentproject/) { get; } | Gets the parent project of the TaskCollection object. |

## Methods

| Name | Description |
| --- | --- |
| [Add](../../aspose.tasks/taskcollection/add/#add)() | Adds new task to project tasks collection on the same outline level of the last task. |
| [Add](../../aspose.tasks/taskcollection/add/#add_1)(RecurringTaskParameters) | Inserts a new task before a task with the specified id and on the same outline level. |
| [Add](../../aspose.tasks/taskcollection/add/#add_2)(string) | Adds a new task to children tasks collection. |
| [Add](../../aspose.tasks/taskcollection/add/#add_4)(Task) | Add the specified task to the instance of the `TaskCollection` class. If ParentProject.CalculationMode is None user should invoke Project.Recalculate() after using this method (It will reschedule all project tasks (start/finish dates, sets early/late dates) and calculate the dependent fields such as slacks, work and cost fields, ids and outline levels). If ParentProject.CalculationMode is Manual the method will calculate only task id, outline level and outline numbers automatically. If ParentProject.CalculationMode is Automatic the method reschedules all project's tasks automatically (start/finish dates, sets early/late dates, calculates slacks, work and cost fields, recalculates ids and outline levels). |
| [Add](../../aspose.tasks/taskcollection/add/#add_3)(string, int) | Adds a new recurring task to children tasks collection. |
| [Contains](../../aspose.tasks/taskcollection/contains/)(Task) | Checks if collection contains specified item. |
| [GetById](../../aspose.tasks/taskcollection/getbyid/)(int) | Returns a task with the specified Id whose ancestor is parent task of this collection . |
| [GetByUid](../../aspose.tasks/taskcollection/getbyuid/)(int) | Returns a task with the specified Uid whose ancestor is parent task of this collection . |
| [GetEnumerator](../../aspose.tasks/taskcollection/getenumerator/)() | Returns an enumerator for this collection. |
| [Insert](../../aspose.tasks/taskcollection/insert/)(int, Task) | This is the stub implementation of IList's Insert method, that only throws NotSupportedException |
| [Remove](../../aspose.tasks/taskcollection/remove/)(Task) | This is the stub implementation of ICollection's Remove method, that only throws NotSupportedException |
| [ToList](../../aspose.tasks/taskcollection/tolist/)() | Converts the TaskCollection object to a list of [`Task`](../task/) objects. |

## Examples

Shows how to work with task collections.

```csharp
var project = new Project();

// the task collection is not read-only and can be extended
Console.WriteLine("Is task collection read - only: " + project.RootTask.Children.IsReadOnly);

// create tasks
var task1 = project.RootTask.Children.Add();
task1.Set(Tsk.Name, "Task 1");
task1.Set(Tsk.Start, new DateTime(2020, 4, 15, 8, 0, 0));
task1.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));
task1.Set(Tsk.Finish, new DateTime(2020, 4, 15, 17, 0, 0));
var task3 = project.RootTask.Children.Add("Task 3");
task3.Set(Tsk.Start, new DateTime(2020, 4, 15, 8, 0, 0));
task3.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));
task3.Set(Tsk.Finish, new DateTime(2020, 4, 15, 17, 0, 0));
var task2 = project.RootTask.Children.Add("Task 2", 2);
task2.Set(Tsk.Start, new DateTime(2020, 4, 15, 8, 0, 0));
task2.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));

// print project tasks
Console.WriteLine("Count of tasks: " + project.RootTask.Children.Count);
foreach (var child in project.RootTask.Children)
{
    Console.WriteLine("Parent Project: " + project.RootTask.ParentProject.Get(Prj.Name));
    Console.WriteLine("Task name: " + child.Get(Tsk.Name));
    Console.WriteLine("Task start: " + child.Get(Tsk.Start));
    Console.WriteLine("Task duration: " + child.Get(Tsk.Duration));
    Console.WriteLine("Task finish: " + child.Get(Tsk.Finish));
    Console.WriteLine();
}

// a task can be taken from the collection by ID
var task1ToEdit = project.RootTask.Children.GetById(1);
task1ToEdit.Set(Tsk.Name, "Task 1 (Edited)");

// or by UID
var taskToEdit2 = project.RootTask.Children.GetByUid(2);
taskToEdit2.Set(Tsk.Name, "Task 2 (Edited)");

// also one can add a recurring task
var parameters = new RecurringTaskParameters
                     {
                         TaskName = "t1",
                         Duration = project.GetDuration(1, TimeUnitType.Day),
                         RecurrencePattern = new DailyRecurrencePattern
                                                 {
                                                     Repetition = new DailyCalendarRepetition { RepetitionInterval = 1 },
                                                     RecurrenceRange = new EndByRecurrenceRange
                                                                           {
                                                                               Start = new DateTime(2020, 4, 13, 8, 0, 0),
                                                                               Finish = new DateTime(2021, 4, 13, 17, 0, 0)
                                                                           }
                                                 }
                     };

// the first task in a sequence is returned
var recurring = project.RootTask.Children.Add(parameters);
Console.WriteLine("Task name: " + recurring.Get(Tsk.Name));

// the collection can be converted into a plain list
List<Task> tasks = project.RootTask.Children.ToList();
foreach (var task in tasks)
{
    task.Delete();
}
```

### See Also

* class [Task](../task/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


