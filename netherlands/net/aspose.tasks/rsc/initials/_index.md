---
title: "Rsc.Initials"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Rsc-veld. De initialen van een resource"
type: docs
weight: 370
url: /nl/net/aspose.tasks/rsc/initials/
---
## Rsc.Initials field

De initialen van een resource.

```csharp
public static readonly Key<string, RscKey> Initials;
```

## Voorbeelden

Toont hoe de eigenschap Rsc.Initials gelezen/geschreven kan worden.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Initials, "R");

Console.WriteLine("Initials: " + resource.Get(Rsc.Initials));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


