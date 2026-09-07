---
title: "TaskLinkCollection.ToList"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo TaskLinkCollection. Converte l'oggetto TaskLinkCollection in un elenco di oggetti TaskLink"
type: docs
weight: 70
url: /it/net/aspose.tasks/tasklinkcollection/tolist/
---
## TaskLinkCollection.ToList method

Converte l'oggetto TaskLinkCollection in un elenco di oggetti [`TaskLink`](../../tasklink/).

```csharp
public List<TaskLink> ToList()
```

### Valore di ritorno

Elenco di oggetti [`TaskLink`](../../tasklink/).

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

* class [TaskLink](../../tasklink/)
* class [TaskLinkCollection](../)
* namespace [Aspose.Tasks](../../tasklinkcollection/)
* assembly [Aspose.Tasks](../../../)


