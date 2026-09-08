---
title: "Rsc.IsNull"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Rsc-veld. Bepaalt of een resource null is."
type: docs
weight: 420
url: /nl/net/aspose.tasks/rsc/isnull/
---
## Rsc.IsNull field

Bepaalt of een resource null is.

```csharp
public static readonly Key<NullableBool, RscKey> IsNull;
```

## Voorbeelden

Toont hoe de eigenschap Rsc.IsNull te lezen/schrijven.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.IsNull, true);

Console.WriteLine("Is Null: " + resource.Get(Rsc.IsNull));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


