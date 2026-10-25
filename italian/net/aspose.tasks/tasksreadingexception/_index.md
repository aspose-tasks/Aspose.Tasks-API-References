---
title: "Classe TasksReadingException"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Aspose.Tasks.TasksReadingException classe. Rappresenta il tipo di eccezione di lettura interno standard"
type: docs
weight: 2540
url: /it/net/aspose.tasks/tasksreadingexception/
---
## TasksReadingException class

Rappresenta il tipo di eccezione interno di lettura standard.

```csharp
public class TasksReadingException : TasksLoggedException
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [LogText](../../aspose.tasks/tasksloggedexception/logtext/) { get; } | Ottiene le informazioni di registrazione dell'eccezione. |
| [Operation](../../aspose.tasks/tasksloggedexception/operation/) { get; } | Ottiene le informazioni sull'operazione dell'eccezione. |

## Esempi

Mostra come gestire le eccezioni di lettura/scrittura del progetto.

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

### Vedi anche

* class [TasksLoggedException](../tasksloggedexception/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


