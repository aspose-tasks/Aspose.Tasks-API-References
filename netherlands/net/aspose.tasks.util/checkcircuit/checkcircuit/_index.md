---
title: "CheckCircuit.CheckCircuit"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "CheckCircuit constructor. Initialiseert een nieuw exemplaar van de CheckCircuit-klasse"
type: docs
weight: 10
url: /nl/net/aspose.tasks.util/checkcircuit/checkcircuit/
---
## CheckCircuit constructor

Initialiseert een nieuw exemplaar van de [`CheckCircuit`](../) klasse.

```csharp
public CheckCircuit()
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

* class [CheckCircuit](../)
* namespace [Aspose.Tasks.Util](../../checkcircuit/)
* assembly [Aspose.Tasks](../../../)


