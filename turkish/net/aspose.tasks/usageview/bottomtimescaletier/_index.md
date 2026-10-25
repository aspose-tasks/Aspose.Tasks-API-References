---
title: "UsageView.BottomTimescaleTier"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "UsageView özelliği. Görünümlerin alt zaman ölçeği katmanının ayarlarını alır veya ayarlar. TimescaleTier"
type: docs
weight: 20
url: /tr/net/aspose.tasks/usageview/bottomtimescaletier/
---
## UsageView.BottomTimescaleTier property

Görünümün alt zaman ölçeği katmanının ayarlarını alır veya ayarlar. [`TimescaleTier`](../../../aspose.tasks.visualization/timescaletier/)

```csharp
public TimescaleTier BottomTimescaleTier { get; set; }
```

## Örnekler

Görünüm ayarlarında tanımlanan zaman ölçeği ayarlarıyla görev kullanım görünümünün nasıl oluşturulacağını gösterir.

```csharp
var project = new Project(DataDir + "TaskUsageView.mpp");

var view = project.Views.ToList()[2] as TaskUsageView;

view.TopTimescaleTier.Unit = TimescaleUnit.None;

view.MiddleTimescaleTier.Unit = TimescaleUnit.Weeks;
view.MiddleTimescaleTier.Label = DateLabel.WeekDddMDd;
view.MiddleTimescaleTier.Count = 1;

view.BottomTimescaleTier.Unit = TimescaleUnit.Days;
view.BottomTimescaleTier.Label = DateLabel.DayMmDd;
view.BottomTimescaleTier.Count = 1;

// SaveOptions'ı tanımlayın ve TaskUsageView zaman ölçeği ayarlarının kullanılmasını belirtin.
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.DefinedInView,
    PresentationFormat = PresentationFormat.TaskUsage
};

project.Save(OutDir + "TaskUsageView_CustomTimescale_out.pdf", options);
```

### Ayrıca Bakınız

* class [TimescaleTier](../../../aspose.tasks.visualization/timescaletier/)
* class [UsageView](../)
* namespace [Aspose.Tasks](../../usageview/)
* assembly [Aspose.Tasks](../../../)


