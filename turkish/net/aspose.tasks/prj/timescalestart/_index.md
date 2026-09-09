---
title: "Prj.TimescaleStart"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Prj alan. Görünümde zaman ölçeğinin başladığı tarih."
type: docs
weight: 740
url: /tr/net/aspose.tasks/prj/timescalestart/
---
## Prj.TimescaleStart field

Görünümdeki zaman ölçeğinin başladığı tarih.

```csharp
public static readonly Key<DateTime, PrjKey> TimescaleStart;
```

## Örnekler

Görünümün başlaması gereken tarihi ayarlamak için zaman ölçeği başlangıç tarihinin nasıl belirleneceğini gösterir.

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Set(Prj.TimescaleStart, new DateTime(2012, 4, 30));

Console.WriteLine("Timescale Start: " + project.Get(Prj.TimescaleStart));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


