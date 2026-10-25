---
title: "Task.SplitParts"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà Task. Ottiene una raccolta SplitPart che rappresenta le porzioni di un'attività"
type: docs
weight: 1110
url: /it/net/aspose.tasks/task/splitparts/
---
## Task.SplitParts property

Ottiene una collezione SplitPart che rappresenta le parti di un'attività.

```csharp
public SplitPartCollection SplitParts { get; }
```

## Esempi

Mostra come visualizzare le parti divise dell'attività.

```csharp
var project = new Project(DataDir + "ViewSplitTasks.mpp");

// Accedi all'attività 
var task = project.RootTask.Children.GetById(4);

// Visualizza le parti divise dell'attività
var collection = task.SplitParts;
foreach (var splitPart in collection)
{
    Console.WriteLine("Start: " + splitPart.Start + "\nFinish: " + splitPart.Finish + "\n");
}
```

### Vedi anche

* class [SplitPartCollection](../../splitpartcollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


