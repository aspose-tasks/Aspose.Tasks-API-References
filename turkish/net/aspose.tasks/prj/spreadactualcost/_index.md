---
title: "Prj.SpreadActualCost"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Prj alanı. Gerçek maliyetlerin durum tarihine yayılıp yayılmayacağını belirler"
type: docs
weight: 660
url: /tr/net/aspose.tasks/prj/spreadactualcost/
---
## Prj.SpreadActualCost field

Gerçek maliyetlerin durum tarihine yayılıp yayılmayacağını belirler.

```csharp
public static readonly Key<NullableBool, PrjKey> SpreadActualCost;
```

## Örnekler

Prj.SpreadActualCost özelliğinin nasıl okunup yazılacağını gösterir.

```csharp
var project = new Project();

project.Set(Prj.SpreadActualCost, true);

Console.WriteLine("Spread Actual Cost: " + project.Get(Prj.SpreadActualCost));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


