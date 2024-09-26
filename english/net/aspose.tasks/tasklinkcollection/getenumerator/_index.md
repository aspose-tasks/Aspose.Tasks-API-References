---
title: TaskLinkCollection.GetEnumerator
second_title: Aspose.Tasks for .NET API Reference
description: TaskLinkCollection method. Returns an enumerator for this collection
type: docs
weight: 50
url: /net/aspose.tasks/tasklinkcollection/getenumerator/
---
## TaskLinkCollection.GetEnumerator method

Returns an enumerator for this collection.

```csharp
public IEnumerator<TaskLink> GetEnumerator()
```

### Return Value

an enumerator for this collection.

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

* class [TaskLink](../../tasklink/)
* class [TaskLinkCollection](../)
* namespace [Aspose.Tasks](../../tasklinkcollection/)
* assembly [Aspose.Tasks](../../../)


