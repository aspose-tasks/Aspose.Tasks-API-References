---
title: "Klasse TaskLinkCollection"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.TaskLinkCollection klasse. Vertegenwoordigt een collectie van Task-objecten"
type: docs
weight: 2420
url: /nl/net/aspose.tasks/tasklinkcollection/
---
## TaskLinkCollection class

Vertegenwoordigt een collectie van [`Task`](../task/) objecten.

```csharp
public class TaskLinkCollection : IList<TaskLink>
```

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [Count](../../aspose.tasks/tasklinkcollection/count/) { get; } | Haalt het aantal objecten op dat in dit `TaskLinkCollection` object zit. |
| [Item](../../aspose.tasks/tasklinkcollection/item/) { get; set; } | Retourneert of stelt het element in op de opgegeven index. |
| [ParentProject](../../aspose.tasks/tasklinkcollection/parentproject/) { get; } | Haalt het bovenliggende project op van het ResourceAssignmentCollection-object. bovenliggend [`Project`](../project/) voor dit object. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| [Add](../../aspose.tasks/tasklinkcollection/add/#add_3)(TaskLink) | Dit is de stub-implementatie van de Add-methode van ICollection, die alleen NotSupportedException gooit. |
| [Add](../../aspose.tasks/tasklinkcollection/add/#add)(Task, Task) | Retourneert een instantie van Finish-Start [`TaskLink`](../tasklink/) die is toegevoegd aan het TaskLinkCollection-object. |
| [Add](../../aspose.tasks/tasklinkcollection/add/#add_1)(Task, Task, TaskLinkType) | Retourneert een instantie van [`TaskLink`](../tasklink/) die is toegevoegd aan het TaskLinkCollection-object. |
| [Add](../../aspose.tasks/tasklinkcollection/add/#add_2)(Task, Task, TaskLinkType, Duration) | Retourneert een instantie van [`TaskLink`](../tasklink/) die is toegevoegd aan het TaskLinkCollection-object. |
| [GetEnumerator](../../aspose.tasks/tasklinkcollection/getenumerator/)() | Retourneert een enumerator voor deze collectie. |
| [Remove](../../aspose.tasks/tasklinkcollection/remove/)(TaskLink) | Verwijdert taakkoppeling uit een project. |
| [ToList](../../aspose.tasks/tasklinkcollection/tolist/)() | Converteert het TaskLinkCollection-object naar een lijst van [`TaskLink`](../tasklink/) objecten. |

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

* class [TaskLink](../tasklink/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


