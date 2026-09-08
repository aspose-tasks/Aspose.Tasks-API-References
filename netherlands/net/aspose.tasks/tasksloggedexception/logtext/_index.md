---
title: "TasksLoggedException.LogText"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "TasksLoggedException eigenschap. Haalt de logboekinformatie van de exceptie op"
type: docs
weight: 10
url: /nl/net/aspose.tasks/tasksloggedexception/logtext/
---
## TasksLoggedException.LogText property

Haalt de logboekinformatie van de uitzondering op.

```csharp
public string LogText { get; }
```

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

* class [TasksLoggedException](../)
* namespace [Aspose.Tasks](../../tasksloggedexception/)
* assembly [Aspose.Tasks](../../../)


