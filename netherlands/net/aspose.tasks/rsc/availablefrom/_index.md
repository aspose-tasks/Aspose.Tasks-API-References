---
title: "Rsc.AvailableFrom"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Rsc-veld. De startdatum waarop een resource beschikbaar is voor werk volgens de eenheden die zijn gespecificeerd voor de huidige periode"
type: docs
weight: 120
url: /nl/net/aspose.tasks/rsc/availablefrom/
---
## Rsc.AvailableFrom field

De startdatum waarop een resource beschikbaar is voor werk volgens de eenheden die zijn gespecificeerd voor de huidige periode.

```csharp
public static readonly Key<DateTime, RscKey> AvailableFrom;
```

## Voorbeelden

Toont hoe de eigenschap Rsc.AvailableFrom gelezen/geschreven kan worden.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.AvailableFrom, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Available From: " + resource.Get(Rsc.AvailableFrom));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


