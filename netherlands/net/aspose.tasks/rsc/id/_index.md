---
title: "Rsc.Id"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Rsc-veld. De positie‑identificatie van een resource binnen de lijst met resources"
type: docs
weight: 350
url: /nl/net/aspose.tasks/rsc/id/
---
## Rsc.Id field

De positie‑identificatie van een resource in de lijst met resources.

```csharp
public static readonly Key<int, RscKey> Id;
```

## Voorbeelden

Toont hoe de eigenschap Rsc.Id gelezen/geschreven kan worden.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Id, 987);

Console.WriteLine("Id: " + resource.Get(Rsc.Id));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


