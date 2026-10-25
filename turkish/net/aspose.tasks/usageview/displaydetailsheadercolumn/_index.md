---
title: "UsageView.DisplayDetailsHeaderColumn"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "UsageView özelliği. Görünümde detay başlık sütununu gösterip göstermeyeceğini belirten bir değeri alır veya ayarlar"
type: docs
weight: 30
url: /tr/net/aspose.tasks/usageview/displaydetailsheadercolumn/
---
## UsageView.DisplayDetailsHeaderColumn property

Görünümde ayrıntı başlık sütununun gösterilip gösterilmeyeceğini belirten bir değeri alır veya ayarlar.

```csharp
public bool DisplayDetailsHeaderColumn { get; set; }
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


