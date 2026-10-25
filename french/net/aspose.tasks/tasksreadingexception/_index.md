---
title: "Classe TasksReadingException"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.TasksReadingException. Représente le type d'exception de lecture interne standard"
type: docs
weight: 2540
url: /fr/net/aspose.tasks/tasksreadingexception/
---
## TasksReadingException class

Représente le type d'exception interne de lecture standard.

```csharp
public class TasksReadingException : TasksLoggedException
```

## Propriétés

| Nom | Description |
| --- | --- |
| [LogText](../../aspose.tasks/tasksloggedexception/logtext/) { get; } | Obtient les informations de journalisation de l'exception. |
| [Operation](../../aspose.tasks/tasksloggedexception/operation/) { get; } | Obtient les informations d'opération de l'exception. |

## Exemples

Montre comment gérer les exceptions de lecture/écriture du projet.

```csharp
try
{
    var project = new Project(DataDir + "project.mpp");
    project.Save(OutDir + "HandleExceptions_out.mpp", SaveFileFormat.Mpp);
}
catch (TasksReadingException ex)
{
    Console.WriteLine("Message: ");
    Console.WriteLine(ex.Message);
    Console.WriteLine("Log: ");
    Console.WriteLine(ex.LogText);
    if (ex.InnerException != null)
    {
        Console.WriteLine("Inner exception message: ");
        Console.WriteLine(ex.InnerException.Message);
    }
}
```

### Voir aussi

* class [TasksLoggedException](../tasksloggedexception/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


