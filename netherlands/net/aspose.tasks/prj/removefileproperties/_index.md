---
title: "Prj.RemoveFileProperties"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Prj-veld. Bepaalt of alle bestandseigenschappen bij het opslaan worden verwijderd"
type: docs
weight: 600
url: /nl/net/aspose.tasks/prj/removefileproperties/
---
## Prj.RemoveFileProperties field

Bepaalt of alle bestands‑eigenschappen bij het opslaan worden verwijderd.

```csharp
public static readonly Key<NullableBool, PrjKey> RemoveFileProperties;
```

## Voorbeelden

Toont hoe de eigenschap Prj.RemoveFileProperties te lezen/schrijven.

```csharp
var project = new Project();

project.Set(Prj.RemoveFileProperties, true);

Console.WriteLine("Remove File Properties: " + project.Get(Prj.RemoveFileProperties));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


