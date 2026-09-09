---
title: "UsageView.DisplayShortDetailHeaderNames"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "UsageView özelliği. Kısa detay başlık adlarının gösterilip gösterilmeyeceğini belirten bir değeri alır veya ayarlar"
type: docs
weight: 40
url: /tr/net/aspose.tasks/usageview/displayshortdetailheadernames/
---
## UsageView.DisplayShortDetailHeaderNames property

Kısa detay başlık adlarının görüntülenip görüntülenmeyeceğini belirten bir değeri alır veya ayarlar.

```csharp
public bool DisplayShortDetailHeaderNames { get; set; }
```

## Örnekler

Görev kullanım görünümünü detaylarla nasıl render edeceğini gösterir.

```csharp
var project = new Project(DataDir + "TaskUsageViewWithDetails.mpp");

// görünümü al
UsageView view = (TaskUsageView)project.DefaultView;

// detay başlık sütunu görüntülenmeyecek
view.DisplayDetailsHeaderColumn = false;
view.RepeatDetailsHeaderOnAllRows = false;
view.DisplayShortDetailHeaderNames = false;
view.AlignDetailsData = HorizontalStringAlignment.Near;
project.Save(OutDir + "task usage1_out.pdf", SaveFileFormat.Pdf);

// detay başlık sütununu görüntüle
view.DisplayDetailsHeaderColumn = true;

// tüm atama satırlarında detay başlığını tekrarla
view.RepeatDetailsHeaderOnAllRows = true;
view.AlignDetailsData = HorizontalStringAlignment.Far;
project.Save(OutDir + "task usage2_out.pdf", SaveFileFormat.Pdf);
```

### Ayrıca Bakınız

* class [UsageView](../)
* namespace [Aspose.Tasks](../../usageview/)
* assembly [Aspose.Tasks](../../../)


