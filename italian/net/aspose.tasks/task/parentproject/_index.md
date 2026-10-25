---
title: "Task.ParentProject"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà Task. Ottiene il progetto padre di un'attività"
type: docs
weight: 930
url: /it/net/aspose.tasks/task/parentproject/
---
## Task.ParentProject property

Ottiene il progetto genitore di un'attività.

```csharp
public Project ParentProject { get; }
```

## Osservazioni

Chiama Project.UpdateReferences per aggiornare queste proprietà.

## Esempi

Mostra come utilizzare il progetto padre dell'attività.

```csharp
var project = new Project();
var task = project.RootTask.Children.Add("Parent");

// Imposta una durata per l'attività utilizzando il tipo di unità di tempo predefinito del progetto.
task.Set(Tsk.Duration, task.ParentProject.GetDuration(1));

Console.WriteLine(task.Get(Tsk.Duration));
```

### Vedi anche

* class [Project](../../project/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


