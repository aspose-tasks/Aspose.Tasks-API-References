---
title: "CheckCircuit.Alg"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "CheckCircuit methode. Controleer of het opgegeven object al verwerkt is"
type: docs
weight: 20
url: /nl/net/aspose.tasks.util/checkcircuit/alg/
---
## CheckCircuit.Alg method

Controleer of het opgegeven object al verwerkt is.

```csharp
public override void Alg(Task el, int level)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| el | Taak | Object om te verwerken. |
| niveau | Int32 | Boomknoopniveau. |

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

* class [Task](../../../aspose.tasks/task/)
* class [CheckCircuit](../)
* namespace [Aspose.Tasks.Util](../../checkcircuit/)
* assembly [Aspose.Tasks](../../../)


