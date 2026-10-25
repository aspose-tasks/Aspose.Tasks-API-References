---
title: "Rsc.MaterialLabel"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Rsc field. De meeteenheid voor de materiaalresource"
type: docs
weight: 440
url: /nl/net/aspose.tasks/rsc/materiallabel/
---
## Rsc.MaterialLabel field

De meeteenheid voor de materiaalresource.

```csharp
public static readonly Key<string, RscKey> MaterialLabel;
```

## Voorbeelden

Toont hoe de eigenschap Rsc.MaterialLabel te lezen/schrijven.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.MaterialLabel, "kg");

Console.WriteLine("Material Label: " + resource.Get(Rsc.MaterialLabel));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


