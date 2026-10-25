---
title: "UsageView.AlignDetailsData"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "UsageView özelliği. Detay verisi hizalamasını alır veya ayarlar"
type: docs
weight: 10
url: /tr/net/aspose.tasks/usageview/aligndetailsdata/
---
## UsageView.AlignDetailsData property

Ayrıntı veri hizalamasını alır veya ayarlar.

```csharp
public HorizontalStringAlignment AlignDetailsData { get; set; }
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

* enum [HorizontalStringAlignment](../../../aspose.tasks.visualization/horizontalstringalignment/)
* class [UsageView](../)
* namespace [Aspose.Tasks](../../usageview/)
* assembly [Aspose.Tasks](../../../)


