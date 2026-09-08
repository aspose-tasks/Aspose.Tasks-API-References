---
title: "Rsc.CostPerUse"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Rsc veld. De kost die ontstaat elke keer dat een resource wordt gebruikt"
type: docs
weight: 240
url: /nl/net/aspose.tasks/rsc/costperuse/
---
## Rsc.CostPerUse field

De kosten die ontstaan elke keer dat een resource wordt gebruikt.

```csharp
public static readonly Key<decimal, RscKey> CostPerUse;
```

## Voorbeelden

Toont hoe de eigenschap Rsc.CostPerUse te lezen/schrijven.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.CostPerUse, 9);

Console.WriteLine("Cost Per Use: " + resource.Get(Rsc.CostPerUse));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


