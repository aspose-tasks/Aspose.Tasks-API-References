---
title: "Rsc.IsCostResource"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Rsc field. Bepaalt of een resource een kostresource is"
type: docs
weight: 390
url: /nl/net/aspose.tasks/rsc/iscostresource/
---
## Rsc.IsCostResource field

Bepaalt of een resource een kostenresource is.

```csharp
public static readonly Key<NullableBool, RscKey> IsCostResource;
```

## Voorbeelden

Toont hoe de eigenschap Rsc.IsCostResource te lezen/schrijven.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.IsCostResource, true);

Console.WriteLine("Is Cost Resource: " + resource.Get(Rsc.IsCostResource));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


