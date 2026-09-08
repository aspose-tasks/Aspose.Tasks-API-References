---
title: "Rsc.Guid"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Rsc veld. Bevat de gegenereerde unieke identificatiecode voor de resource"
type: docs
weight: 310
url: /nl/net/aspose.tasks/rsc/guid/
---
## Rsc.Guid field

Bevat de gegenereerde unieke identificatiecode voor de resource.

```csharp
public static readonly Key<string, RscKey> Guid;
```

## Voorbeelden

Toont hoe de eigenschap Rsc.Guid te lezen/schrijven.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Guid, "1385689c-2dd1-4114-935b-054beb6fbbbe");

Console.WriteLine("Guid: " + resource.Get(Rsc.Guid));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


