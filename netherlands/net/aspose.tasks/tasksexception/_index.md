---
title: "Klasse TasksException"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.TasksException‑klasse. Vertegenwoordigt het standaard interne exceptietype"
type: docs
weight: 2520
url: /nl/net/aspose.tasks/tasksexception/
---
## TasksException class

Stelt het standaard interne exceptietype voor.

```csharp
public class TasksException : ApplicationException
```

## Voorbeelden

Toont hoe je een gebroken projectstructuur kunt detecteren.

```csharp
var project = new Project(DataDir + "ParentChildTasks.mpp");

// controleer de projectstructuur.
// De <see cref=\"TasksException\"> wordt gegooid als de projectstructuur onjuist is.
try
{
    TaskUtils.Apply(project.RootTask, new CheckCircuit(), 0);
}
catch (TasksException ex)
{
    Console.WriteLine(ex);
}
```

### Zie ook

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


