---
title: "Klasse CheckCircuit"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.Util.CheckCircuit-klasse. Controleert een boom van taken of deze een circuit bevat"
type: docs
weight: 2680
url: /nl/net/aspose.tasks.util/checkcircuit/
---
## CheckCircuit class

Controleert een boom (van taken) of deze een circuit bevat.

```csharp
public class CheckCircuit : TreeAlgorithmBase<Task>
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [CheckCircuit](checkcircuit/)() | Initialiseert een nieuw exemplaar van de `CheckCircuit`-klasse. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| override [Alg](../../aspose.tasks.util/checkcircuit/alg/)(Task, int) | Controleer of het opgegeven object al verwerkt is. |
| virtual [PostAlg](../../aspose.tasks.util/treealgorithmbase-1/postalg/)(Task, int) |  |
| virtual [PreAlg](../../aspose.tasks.util/treealgorithmbase-1/prealg/)(Task, int) |  |

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

* class [TreeAlgorithmBase&lt;T&gt;](../treealgorithmbase-1/)
* class [Task](../../aspose.tasks/task/)
* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


