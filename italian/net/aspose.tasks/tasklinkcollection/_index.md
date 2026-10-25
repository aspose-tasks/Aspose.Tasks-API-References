---
title: "Classe TaskLinkCollection"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.TaskLinkCollection. Rappresenta una raccolta di oggetti Task."
type: docs
weight: 2420
url: /it/net/aspose.tasks/tasklinkcollection/
---
## TaskLinkCollection class

Rappresenta una raccolta di oggetti [`Task`](../task/).

```csharp
public class TaskLinkCollection : IList<TaskLink>
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Count](../../aspose.tasks/tasklinkcollection/count/) { get; } | Ottiene il numero di oggetti contenuti in questo oggetto `TaskLinkCollection`. |
| [Item](../../aspose.tasks/tasklinkcollection/item/) { get; set; } | Restituisce o imposta l'elemento all'indice specificato. |
| [ParentProject](../../aspose.tasks/tasklinkcollection/parentproject/) { get; } | Ottiene il progetto padre dell'oggetto ResourceAssignmentCollection. progetto padre [`Project`](../project/) per questo oggetto. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Add](../../aspose.tasks/tasklinkcollection/add/#add_3)(TaskLink) | Questa è l'implementazione stub del metodo Add di ICollection, che lancia solo NotSupportedException |
| [Add](../../aspose.tasks/tasklinkcollection/add/#add)(Task, Task) | Restituisce un'istanza di Finish-Start [`TaskLink`](../tasklink/) che è stata aggiunta all'oggetto TaskLinkCollection. |
| [Add](../../aspose.tasks/tasklinkcollection/add/#add_1)(Task, Task, TaskLinkType) | Restituisce un'istanza di [`TaskLink`](../tasklink/) che è stata aggiunta all'oggetto TaskLinkCollection. |
| [Add](../../aspose.tasks/tasklinkcollection/add/#add_2)(Task, Task, TaskLinkType, Duration) | Restituisce un'istanza di [`TaskLink`](../tasklink/) che è stata aggiunta all'oggetto TaskLinkCollection. |
| [GetEnumerator](../../aspose.tasks/tasklinkcollection/getenumerator/)() | Restituisce un enumeratore per questa collezione. |
| [Remove](../../aspose.tasks/tasklinkcollection/remove/)(TaskLink) | Rimuove il collegamento di attività da un progetto. |
| [ToList](../../aspose.tasks/tasklinkcollection/tolist/)() | Converte l'oggetto TaskLinkCollection in un elenco di oggetti [`TaskLink`](../tasklink/). |

## Esempi

Mostra come lavorare con collezioni di collegamenti di attività.

```csharp
var project = new Project(DataDir + "SampleProject.mpp");

// ottieni attività
var task1 = project.RootTask.Children.GetById(1);
var task2 = project.RootTask.Children.GetById(2);
var task3 = project.RootTask.Children.GetById(3);
var task4 = project.RootTask.Children.GetById(4);
var task5 = project.RootTask.Children.GetById(5);

// collega le attività
project.TaskLinks.Add(task1, task2);
project.TaskLinks.Add(task2, task3, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task3, task4, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task4, task5, TaskLinkType.FinishToStart, project.GetDuration(1, TimeUnitType.Day));
project.TaskLinks.Add(task2, task5, TaskLinkType.FinishToStart, project.GetDuration(2, TimeUnitType.Day));

// stampa i collegamenti tra le attività
Console.WriteLine("Print task links of " + project.TaskLinks.ParentProject.Get(Prj.Name) + " project.");
Console.WriteLine("Task links count: " + project.TaskLinks.Count);
foreach (var link in project.TaskLinks)
{
    Console.WriteLine("From ID = " + link.PredTask.Get(Tsk.Id) + " => To ID = " + link.SuccTask.Get(Tsk.Id));
    Console.WriteLine();
}

// modifica il collegamento tramite accesso per indice
project.TaskLinks[0].LagFormat = TimeUnitType.Hour;

// rimuovi tutti i collegamenti di attività
List<TaskLink> taskLinks = project.TaskLinks.ToList();
foreach (var link in taskLinks)
{
    project.TaskLinks.Remove(link);
}
```

### Vedi anche

* class [TaskLink](../tasklink/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


