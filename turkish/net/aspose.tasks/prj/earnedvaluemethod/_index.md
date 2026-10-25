---
title: "Prj.EarnedValueMethod"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Prj alanı. Kazanılmış değeri hesaplamak için varsayılan yöntem"
type: docs
weight: 310
url: /tr/net/aspose.tasks/prj/earnedvaluemethod/
---
## Prj.EarnedValueMethod field

Kazanılmış değeri hesaplamak için varsayılan yöntem.

```csharp
public static readonly Key<EarnedValueMethodType, PrjKey> EarnedValueMethod;
```

## Örnekler

Prj.EarnedValueMethod özelliğinin nasıl okunup yazılacağını gösterir.

```csharp
var project = new Project();

project.Set(Prj.EarnedValueMethod, EarnedValueMethodType.PhysicalPercentComplete);

Console.WriteLine("Earned Value Method: " + project.Get(Prj.EarnedValueMethod));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [EarnedValueMethodType](../../earnedvaluemethodtype/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


