---
title: "Prj.Guid"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Prj-veld. De GUID van het project"
type: docs
weight: 360
url: /nl/net/aspose.tasks/prj/guid/
---
## Prj.Guid field

De GUID van het project.

```csharp
public static readonly Key<Guid, PrjKey> Guid;
```

## Voorbeelden

Toont hoe de eigenschap Prj.Guid te lezen/schrijven.

```csharp
var project = new Project();

project.Set(Prj.Guid, new Guid("efcc0d63-d8e0-4a34-9f3e-9f973f50238a"));

Console.WriteLine("Guid: " + project.Get(Prj.Guid));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


