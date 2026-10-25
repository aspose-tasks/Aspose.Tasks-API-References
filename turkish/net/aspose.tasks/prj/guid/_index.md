---
title: "Prj.Guid"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Prj alanı. Projenin GUID'si"
type: docs
weight: 360
url: /tr/net/aspose.tasks/prj/guid/
---
## Prj.Guid field

Projenin GUID'si.

```csharp
public static readonly Key<Guid, PrjKey> Guid;
```

## Örnekler

Prj.Guid özelliğinin nasıl okunup yazılacağını gösterir.

```csharp
var project = new Project();

project.Set(Prj.Guid, new Guid("efcc0d63-d8e0-4a34-9f3e-9f973f50238a"));

Console.WriteLine("Guid: " + project.Get(Prj.Guid));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


