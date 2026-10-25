---
title: "Resource.Baselines"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà Resource. Ottiene un'istanza di BaselineCollection per questo oggetto. I valori di baseline per una risorsa"
type: docs
weight: 160
url: /it/net/aspose.tasks/resource/baselines/
---
## Resource.Baselines property

Ottiene un'istanza di BaselineCollection per questo oggetto. I valori di baseline per una risorsa.

```csharp
public BaselineCollection Baselines { get; }
```

## Esempi

Mostra come leggere le baseline della risorsa.

```csharp
var project = new Project(DataDir + "Baselines2010.mpp");

foreach (var resource in project.Resources)
{
    foreach (var baseline in resource.Baselines)
    {
        Console.WriteLine("BaselineNumber: " + baseline.BaselineNumber);
        Console.WriteLine("Bcwp: " + baseline.Bcwp);
        Console.WriteLine("Bcws: " + baseline.Bcws);
        Console.WriteLine("Cost: " + baseline.Cost);
        Console.WriteLine("Work: " + baseline.Work);
    }
}
```

### Vedi anche

* class [BaselineCollection](../../baselinecollection/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


