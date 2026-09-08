---
title: "Rsc.Uid"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Rsc veld. De unieke identificatie van een resource."
type: docs
weight: 670
url: /nl/net/aspose.tasks/rsc/uid/
---
## Rsc.Uid field

De unieke identifier van een resource.

```csharp
public static readonly Key<int, RscKey> Uid;
```

## Voorbeelden

Toont hoe de Rsc.Uid eigenschap te lezen/schrijven.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Uid, 99);

Console.WriteLine("Uid: " + resource.Get(Rsc.Uid));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


