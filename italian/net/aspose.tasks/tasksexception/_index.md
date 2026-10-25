---
title: "Classe TasksException"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.TasksException. Rappresenta il tipo di eccezione interno standard"
type: docs
weight: 2520
url: /it/net/aspose.tasks/tasksexception/
---
## TasksException class

Rappresenta il tipo di eccezione interno standard.

```csharp
public class TasksException : ApplicationException
```

## Esempi

Mostra come rilevare la struttura del progetto rotta.

```csharp
var project = new Project(DataDir + "ParentChildTasks.mpp");

// verifica la struttura del progetto.
// Il <see cref=\"TasksException\"> verrà generato se la struttura del progetto è errata.
try
{
    TaskUtils.Apply(project.RootTask, new CheckCircuit(), 0);
}
catch (TasksException ex)
{
    Console.WriteLine(ex);
}
```

### Vedi anche

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


