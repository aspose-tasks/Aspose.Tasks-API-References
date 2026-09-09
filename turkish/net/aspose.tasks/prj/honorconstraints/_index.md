---
title: "Prj.HonorConstraints"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Prj alan. Görevlerin kısıtlama tarihlerine uyup uymayacağını belirler."
type: docs
weight: 370
url: /tr/net/aspose.tasks/prj/honorconstraints/
---
## Prj.HonorConstraints field

Görevlerin kısıtlama tarihlerini göz önünde bulundurup bulundurmayacağını belirler.

```csharp
public static readonly Key<NullableBool, PrjKey> HonorConstraints;
```

## Örnekler

Prj.HonorConstraints özelliğini nasıl okuyup yazacağınızı gösterir.

```csharp
var project = new Project();

project.Set(Prj.HonorConstraints, true);

Console.WriteLine("Honor Constraints: " + project.Get(Prj.HonorConstraints));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


