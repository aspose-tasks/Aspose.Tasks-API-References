---
title: "Classe TasksException"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.TasksException. Représente le type d'exception interne standard"
type: docs
weight: 2520
url: /fr/net/aspose.tasks/tasksexception/
---
## TasksException class

Représente le type d'exception interne standard.

```csharp
public class TasksException : ApplicationException
```

## Exemples

Montre comment détecter la structure du projet cassée.

```csharp
var project = new Project(DataDir + "ParentChildTasks.mpp");

// vérifier la structure du projet.
// Le <see cref="TasksException"> sera levé si la structure du projet est incorrecte.
try
{
    TaskUtils.Apply(project.RootTask, new CheckCircuit(), 0);
}
catch (TasksException ex)
{
    Console.WriteLine(ex);
}
```

### Voir aussi

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


