---
title: "Prj.SpreadPercentComplete"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Prj alanı. Yüzde tamamlamanın durum tarihine yayılıp yayılmayacağını belirler"
type: docs
weight: 670
url: /tr/net/aspose.tasks/prj/spreadpercentcomplete/
---
## Prj.SpreadPercentComplete field

Tamamlanma yüzdesinin durum tarihine yayılıp yayılmayacağını belirler.

```csharp
public static readonly Key<NullableBool, PrjKey> SpreadPercentComplete;
```

## Örnekler

Prj.SpreadPercentComplete özelliğinin nasıl okunup yazılacağını gösterir.

```csharp
var project = new Project();

project.Set(Prj.SpreadPercentComplete, true);

Console.WriteLine("Spread Percent Complete: " + project.Get(Prj.SpreadPercentComplete));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


