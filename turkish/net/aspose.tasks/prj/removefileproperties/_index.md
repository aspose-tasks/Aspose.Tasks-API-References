---
title: "Prj.RemoveFileProperties"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Prj alanı. Kaydetme sırasında tüm dosya özelliklerinin kaldırılıp kaldırılmayacağını belirler"
type: docs
weight: 600
url: /tr/net/aspose.tasks/prj/removefileproperties/
---
## Prj.RemoveFileProperties field

Kaydedildiğinde tüm dosya özelliklerinin kaldırılıp kaldırılmayacağını belirler.

```csharp
public static readonly Key<NullableBool, PrjKey> RemoveFileProperties;
```

## Örnekler

Prj.RemoveFileProperties özelliğinin nasıl okunup yazılacağını gösterir.

```csharp
var project = new Project();

project.Set(Prj.RemoveFileProperties, true);

Console.WriteLine("Remove File Properties: " + project.Get(Prj.RemoveFileProperties));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


