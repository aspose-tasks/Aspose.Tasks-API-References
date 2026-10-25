---
title: "Klasse TasksReadingException"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.TasksReadingException klasse. Vertegenwoordigt het standaard interne leesfouttype"
type: docs
weight: 2540
url: /nl/net/aspose.tasks/tasksreadingexception/
---
## TasksReadingException class

Stelt het standaard interne leesexceptietype voor.

```csharp
public class TasksReadingException : TasksLoggedException
```

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [LogText](../../aspose.tasks/tasksloggedexception/logtext/) { get; } | Haalt de logboekinformatie van de uitzondering op. |
| [Operation](../../aspose.tasks/tasksloggedexception/operation/) { get; } | Haalt de operationele informatie van de uitzondering op. |

## Voorbeelden

Toont hoe lees-/schrijffouten van een project af te handelen.

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

### Zie ook

* class [TasksLoggedException](../tasksloggedexception/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


