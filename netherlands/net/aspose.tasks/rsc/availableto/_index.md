---
title: "Rsc.AvailableTo"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Rsc-veld. De einddatum waarop een resource beschikbaar is voor werk volgens de eenheden die zijn gespecificeerd voor de huidige periode"
type: docs
weight: 130
url: /nl/net/aspose.tasks/rsc/availableto/
---
## Rsc.AvailableTo field

De einddatum waarop een resource beschikbaar is voor werk volgens de eenheden die zijn gespecificeerd voor de huidige periode.

```csharp
public static readonly Key<DateTime, RscKey> AvailableTo;
```

## Voorbeelden

Toont hoe de eigenschap Rsc.AvailableTo gelezen/geschreven kan worden.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.AvailableTo, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Available To: " + resource.Get(Rsc.AvailableTo));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


