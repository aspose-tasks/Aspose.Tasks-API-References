---
title: "Prj.SpreadActualCost"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Prj. Determina se i costi effettivi sono distribuiti alla data di stato"
type: docs
weight: 660
url: /it/net/aspose.tasks/prj/spreadactualcost/
---
## Prj.SpreadActualCost field

Determina se i costi effettivi vengono distribuiti fino alla data di stato.

```csharp
public static readonly Key<NullableBool, PrjKey> SpreadActualCost;
```

## Esempi

Mostra come leggere/scrivere la proprietà Prj.SpreadActualCost.

```csharp
var project = new Project();

project.Set(Prj.SpreadActualCost, true);

Console.WriteLine("Spread Actual Cost: " + project.Get(Prj.SpreadActualCost));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


