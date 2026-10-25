---
title: "Rsc.IsEnterprise"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Rsc-veld. Toont of een resource uit de enterprise‑resourcepool komt (true) of uit de lokale resourcepool (false)."
type: docs
weight: 400
url: /nl/net/aspose.tasks/rsc/isenterprise/
---
## Rsc.IsEnterprise field

Toont of een resource afkomstig is uit de bedrijfsresource‑pool (true) of de lokale resource‑pool (false).

```csharp
public static readonly Key<NullableBool, RscKey> IsEnterprise;
```

## Voorbeelden

Toont hoe de eigenschap Rsc.IsEnterprise te lezen/schrijven.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.IsEnterprise, true);

Console.WriteLine("Is Enterprise: " + resource.Get(Rsc.IsEnterprise));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


