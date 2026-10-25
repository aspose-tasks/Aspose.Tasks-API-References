---
title: "Notities"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "De tekstnotities die aan een resource zijn gekoppeld."
type: docs
weight: 470
url: /nl/net/aspose.tasks/rsc/notes/
---
## Rsc.Notes field

De tekstnotities die aan een resource zijn gekoppeld.

```csharp
public static readonly Key<string, RscKey> Notes;
```

### Voorbeelden

Toont hoe de Rsc.Notes eigenschap te lezen/schrijven.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Notes, "Resource Notes");

Console.WriteLine("Notes: " + resource.Get(Rsc.Notes));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2)
* enum [RscKey](../../rsckey)
* class [Rsc](../../rsc)
* namespace [Aspose.Tasks](../../rsc)
* assembly [Aspose.Tasks](../../../)

<!-- NIET BEWERKEN: gegenereerd door xmldocmd voor Aspose.Tasks.dll -->
