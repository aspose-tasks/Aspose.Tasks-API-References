---
title: Class TaskLinkCollection
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.TaskLinkCollection class. Represents a collection of Task objects
type: docs
weight: 2390
url: /net/aspose.tasks/tasklinkcollection/
---
## TaskLinkCollection class

Represents a collection of [`Task`](../task/) objects.

```csharp
public class TaskLinkCollection : IList<TaskLink>
```

## Properties

| Name | Description |
| --- | --- |
| [Count](../../aspose.tasks/tasklinkcollection/count/) { get; } | Gets the number of objects contained in this `TaskLinkCollection` object. |
| [Item](../../aspose.tasks/tasklinkcollection/item/) { get; set; } | Returns or sets the element at the specified index. |
| [ParentProject](../../aspose.tasks/tasklinkcollection/parentproject/) { get; } | Gets the parent project of the ResourceAssignmentCollection object. parent [`Project`](../project/) for this object. |

## Methods

| Name | Description |
| --- | --- |
| [Add](../../aspose.tasks/tasklinkcollection/add/#add_3)(TaskLink) | This is the stub implementation of ICollection's Add method, that only throws NotSupportedException |
| [Add](../../aspose.tasks/tasklinkcollection/add/#add)(Task, Task) | Returns an instance of Finish-Start [`TaskLink`](../tasklink/) which has been added to the TaskLinkCollection object. |
| [Add](../../aspose.tasks/tasklinkcollection/add/#add_1)(Task, Task, TaskLinkType) | Returns an instance of [`TaskLink`](../tasklink/) which has been added to the TaskLinkCollection object. |
| [Add](../../aspose.tasks/tasklinkcollection/add/#add_2)(Task, Task, TaskLinkType, Duration) | Returns an instance of [`TaskLink`](../tasklink/) which has been added to the TaskLinkCollection object. |
| [GetEnumerator](../../aspose.tasks/tasklinkcollection/getenumerator/)() | Returns an enumerator for this collection. |
| [Remove](../../aspose.tasks/tasklinkcollection/remove/)(TaskLink) | Removes task link from a project. |
| [ToList](../../aspose.tasks/tasklinkcollection/tolist/)() | Converts the TaskLinkCollection object to a list of [`TaskLink`](../tasklink/) objects. |

## Examples

Shows how to work with task link collections.

```csharp
var project = new Project(DataDir + "SampleProject.mpp");

// get tasks
var task1 = project.RootTask.Children.GetById(1);
var task2 = project.RootTask.Children.GetById(2);
var task3 = project.RootTask.Children.GetById(3);
var task4 = project.RootTask.Children.GetById(4);
var task5 = project.RootTask.Children.GetById(5);

// link the tasks
project.TaskLinks.Add(task1, task2);
project.TaskLinks.Add(task2, task3, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task3, task4, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task4, task5, TaskLinkType.FinishToStart, project.GetDuration(1, TimeUnitType.Day));
project.TaskLinks.Add(task2, task5, TaskLinkType.FinishToStart, project.GetDuration(2, TimeUnitType.Day));

// print links among the tasks
Console.WriteLine("Print task links of " + project.TaskLinks.ParentProject.Get(Prj.Name) + " project.");
Console.WriteLine("Task links count: " + project.TaskLinks.Count);
foreach (var link in project.TaskLinks)
{
    Console.WriteLine("From ID = " + link.PredTask.Get(Tsk.Id) + " => To ID = " + link.SuccTask.Get(Tsk.Id));
    Console.WriteLine();
}

// edit link by index access
project.TaskLinks[0].LagFormat = TimeUnitType.Hour;

// remove all task links
List<TaskLink> taskLinks = project.TaskLinks.ToList();
foreach (var link in taskLinks)
{
    project.TaskLinks.Remove(link);
}
```

### See Also

* class [TaskLink](../tasklink/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


