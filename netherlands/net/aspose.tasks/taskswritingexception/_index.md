---
title: "Klasse TasksWritingException"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.TasksWritingException klasse. Vertegenwoordigt het standaard interne schrijffouttype"
type: docs
weight: 2560
url: /nl/net/aspose.tasks/taskswritingexception/
---
## TasksWritingException class

Stelt het standaard interne schrijfeceptietype voor.

```csharp
public class TasksWritingException : TasksLoggedException
```

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [LogText](../../aspose.tasks/tasksloggedexception/logtext/) { get; } | Haalt de logboekinformatie van de uitzondering op. |
| [Operation](../../aspose.tasks/tasksloggedexception/operation/) { get; } | Haalt de operationele informatie van de uitzondering op. |

## Voorbeelden

Toont hoe logtekst en type fout gelezen moeten worden om problemen met MPP-export te controleren.

```csharp
try
{
    var project = new Project(DataDir + "PrintTaskWritingException.mpp");

    // exporteer het project als een MPP-bestand
    project.Save(OutDir + "PrintTaskWritingException_out.MPP", SaveFileFormat.Mpp);
}
catch (TasksWritingException ex)
{
    Console.WriteLine("Exception Operation: " + ex.Operation);
    Console.WriteLine("Exception Log Text: ");
    Console.WriteLine(ex.LogText);
}
```

### Zie ook

* class [TasksLoggedException](../tasksloggedexception/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


