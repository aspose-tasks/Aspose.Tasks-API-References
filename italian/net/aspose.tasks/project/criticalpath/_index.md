---
title: "Project.CriticalPath"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà di Project. Ottiene una collezione che contiene un elenco di attività Critical che compongono il Critical Path di questo progetto. Questa è un'operazione On dove n è il numero di attività nel progetto"
type: docs
weight: 180
url: /it/net/aspose.tasks/project/criticalpath/
---
## Project.CriticalPath property

Ottiene una collezione che contiene un elenco di attività Critical che compongono il Critical Path di questo progetto. Questa è un'operazione O(n), dove n è il numero di attività nel progetto.

```csharp
public TaskCollection CriticalPath { get; }
```

### Valore di ritorno

una collezione che rappresenta un elenco di tutte le attività critical.

## Esempi

Mostra come calcolare un critical path del progetto.

```csharp
var project = new Project()
{
    CalculationMode = CalculationMode.Automatic
};

var subtask1 = project.RootTask.Children.Add("1");
var subtask2 = project.RootTask.Children.Add("2");
project.TaskLinks.Add(subtask1, subtask2, TaskLinkType.FinishToStart);

project.RootTask.Children.Add("3");

// Visualizza il critical path ora
foreach (var task in project.CriticalPath)
{
    Console.WriteLine(task.Get(Tsk.Id) + "  " + task.Get(Tsk.Name));
    Console.WriteLine(task.Get(Tsk.Start));
    Console.WriteLine(task.Get(Tsk.Finish) + "\n");
}
```

### Vedi anche

* class [TaskCollection](../../taskcollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


