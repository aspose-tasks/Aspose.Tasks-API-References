---
title: "Task.Delete"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo Task. Elimina un task dalla raccolta di task del progetto padre e da tutte le sue assegnazioni"
type: docs
weight: 1320
url: /it/net/aspose.tasks/task/delete/
---
## Task.Delete method

Elimina un'attività dalla collezione di attività del progetto principale e tutte le sue assegnazioni.

```csharp
public void Delete()
```

## Esempi

Mostra come eliminare un task.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

Console.WriteLine("Number of tasks: " + project.RootTask.Children.Count);

// elimina un task
task.Delete();

Console.WriteLine("Number of tasks: " + project.RootTask.Children.Count);
```

### Vedi anche

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


