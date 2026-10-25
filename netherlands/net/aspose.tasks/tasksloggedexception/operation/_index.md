---
title: "TasksLoggedException.Operation"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "TasksLoggedException eigenschap. Haalt de informatie over de exceptie‑operatie op"
type: docs
weight: 20
url: /nl/net/aspose.tasks/tasksloggedexception/operation/
---
## TasksLoggedException.Operation property

Haalt de operationele informatie van de uitzondering op.

```csharp
public string Operation { get; }
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


