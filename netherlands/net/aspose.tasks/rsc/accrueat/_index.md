---
title: "Rsc.AccrueAt"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Rsc veld. Bepaalt hoe en wanneer standaard- en overurenkosten van een resource in rekening worden gebracht of worden toegerekend aan de kosten van een taak"
type: docs
weight: 10
url: /nl/net/aspose.tasks/rsc/accrueat/
---
## Rsc.AccrueAt field

Bepaalt hoe en wanneer standaard- en overurenkosten van resources in rekening worden gebracht, of worden toegerekend, aan de kosten van een taak.

```csharp
public static readonly Key<CostAccrualType, RscKey> AccrueAt;
```

## Voorbeelden

Toont hoe de eigenschap Rsc.AccrueAt te lezen/schrijven.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.AccrueAt, CostAccrualType.End);

Console.WriteLine("Accrue At: " + resource.Get(Rsc.AccrueAt));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [CostAccrualType](../../costaccrualtype/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


