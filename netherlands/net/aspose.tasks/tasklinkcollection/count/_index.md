---
title: "TaskLinkCollection.Count"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "TaskLinkCollection-eigenschap. Geeft het aantal objecten terug dat in dit TaskLinkCollection object is opgenomen."
type: docs
weight: 10
url: /nl/net/aspose.tasks/tasklinkcollection/count/
---
## TaskLinkCollection.Count property

Geeft het aantal objecten terug dat in dit [`TaskLinkCollection`](../) object is opgenomen.

```csharp
public int Count { get; }
```

## Voorbeelden

Toont hoe te werken met taakkoppelingscollecties.

```csharp
var project = new Project(DataDir + "SampleProject.mpp");

// haal taken op
var task1 = project.RootTask.Children.GetById(1);
var task2 = project.RootTask.Children.GetById(2);
var task3 = project.RootTask.Children.GetById(3);
var task4 = project.RootTask.Children.GetById(4);
var task5 = project.RootTask.Children.GetById(5);

// koppel de taken
project.TaskLinks.Add(task1, task2);
project.TaskLinks.Add(task2, task3, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task3, task4, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task4, task5, TaskLinkType.FinishToStart, project.GetDuration(1, TimeUnitType.Day));
project.TaskLinks.Add(task2, task5, TaskLinkType.FinishToStart, project.GetDuration(2, TimeUnitType.Day));

// print koppelingen tussen de taken
Console.WriteLine("Print task links of " + project.TaskLinks.ParentProject.Get(Prj.Name) + " project.");
Console.WriteLine("Task links count: " + project.TaskLinks.Count);
foreach (var link in project.TaskLinks)
{
    Console.WriteLine("From ID = " + link.PredTask.Get(Tsk.Id) + " => To ID = " + link.SuccTask.Get(Tsk.Id));
    Console.WriteLine();
}

// bewerk koppeling via indextoegang
project.TaskLinks[0].LagFormat = TimeUnitType.Hour;

// verwijder alle taakkoppelingen
List<TaskLink> taskLinks = project.TaskLinks.ToList();
foreach (var link in taskLinks)
{
    project.TaskLinks.Remove(link);
}
```

### Zie ook

* class [TaskLinkCollection](../)
* namespace [Aspose.Tasks](../../tasklinkcollection/)
* assembly [Aspose.Tasks](../../../)


