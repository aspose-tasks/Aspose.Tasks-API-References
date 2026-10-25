---
title: "Rsc.IsGeneric"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Rsc-veld. Bepaalt of een resource generiek is of niet."
type: docs
weight: 410
url: /nl/net/aspose.tasks/rsc/isgeneric/
---
## Rsc.IsGeneric field

Bepaalt of een resource generiek is of niet.

```csharp
public static readonly Key<NullableBool, RscKey> IsGeneric;
```

## Voorbeelden

Toont hoe u de eigenschap Rsc.IsGeneric kunt lezen/schrijven.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.IsGeneric, true);

Console.WriteLine("Is Generic: " + resource.Get(Rsc.IsGeneric));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


