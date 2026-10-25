---
title: "Rsc.Inactive"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Rsc-veld. Bepaalt of een resource inactief is gemaakt door een gebruiker met administratieve rechten"
type: docs
weight: 360
url: /nl/net/aspose.tasks/rsc/inactive/
---
## Rsc.Inactive field

Bepaalt of een resource inactief is gemaakt door een gebruiker met administratieve rechten.

```csharp
public static readonly Key<NullableBool, RscKey> Inactive;
```

## Voorbeelden

Toont hoe de eigenschap Rsc.Inactive te lezen/schrijven.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Inactive, true);

Console.WriteLine("Inactive: " + resource.Get(Rsc.Inactive));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


