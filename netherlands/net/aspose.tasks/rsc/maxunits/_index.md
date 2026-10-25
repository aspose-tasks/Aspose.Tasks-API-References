---
title: "Rsc.MaxUnits"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Rsc-veld. Het maximale aantal eenheden dat de maximale capaciteit vertegenwoordigt waarvoor een resource beschikbaar is om taken uit te voeren gedurende de huidige periode."
type: docs
weight: 450
url: /nl/net/aspose.tasks/rsc/maxunits/
---
## Rsc.MaxUnits field

Het maximale aantal eenheden dat de maximale capaciteit weergeeft waarvoor een resource beschikbaar is om taken uit te voeren gedurende de huidige periode.

```csharp
public static readonly Key<double, RscKey> MaxUnits;
```

## Voorbeelden

Toont hoe u de eigenschap Rsc.MaxUnits kunt lezen/schrijven.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.MaxUnits, 2);

Console.WriteLine("Max Units: " + resource.Get(Rsc.MaxUnits));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


