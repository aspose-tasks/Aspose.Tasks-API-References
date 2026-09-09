---
title: "Prj.TimescaleFinish"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Prj alan. Görünümde zaman ölçeğinin bittiği tarih."
type: docs
weight: 730
url: /tr/net/aspose.tasks/prj/timescalefinish/
---
## Prj.TimescaleFinish field

Görünümdeki zaman ölçeğinin bittiği tarih.

```csharp
public static readonly Key<DateTime, PrjKey> TimescaleFinish;
```

## Örnekler

Prj.TimescaleFinish özelliğini nasıl okuyup yazacağınızı gösterir.

```csharp
var project = new Project();

project.Set(Prj.TimescaleFinish, new DateTime(2020, 4, 10, 9, 0, 0));

Console.WriteLine("Timescale Finish: " + project.Get(Prj.TimescaleFinish));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


