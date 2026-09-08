---
title: "Rsc.CanLevel"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Rsc veld. Bepaalt of resource-leveling kan worden uitgevoerd op een resource"
type: docs
weight: 200
url: /nl/net/aspose.tasks/rsc/canlevel/
---
## Rsc.CanLevel field

Bepaalt of resource-leveling kan worden uitgevoerd op een resource.

```csharp
public static readonly Key<NullableBool, RscKey> CanLevel;
```

## Voorbeelden

Toont hoe de eigenschap Rsc.CanLevel te lezen/schrijven.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.CanLevel, true);

Console.WriteLine("Can Level: " + resource.Get(Rsc.CanLevel));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


