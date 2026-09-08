---
title: "Rsc.Type"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Rsc-veld. Het type van een resource."
type: docs
weight: 660
url: /nl/net/aspose.tasks/rsc/type/
---
## Rsc.Type field

Het type van een resource.

```csharp
public static readonly Key<ResourceType, RscKey> Type;
```

## Voorbeelden

Toont hoe de eigenschap Rsc.Type te lezen/schrijven.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Type, ResourceType.Work);

Console.WriteLine("Type: " + resource.Get(Rsc.Type));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [ResourceType](../../resourcetype/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


