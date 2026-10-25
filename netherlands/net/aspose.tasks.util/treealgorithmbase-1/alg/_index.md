---
title: "TreeAlgorithmBase1.Alg"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "TreeAlgorithmBase-methode. Verwerkt een knoop in een boom"
type: docs
weight: 10
url: /nl/net/aspose.tasks.util/treealgorithmbase-1/alg/
---
## TreeAlgorithmBase&lt;T&gt;.Alg method

Verwerkt een knoop van een boom.

```csharp
public abstract void Alg(T el, int level)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| el | T | Knoop om te verwerken. |
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

* class [TreeAlgorithmBase&lt;T&gt;](../)
* namespace [Aspose.Tasks.Util](../../treealgorithmbase-1/)
* assembly [Aspose.Tasks](../../../)


