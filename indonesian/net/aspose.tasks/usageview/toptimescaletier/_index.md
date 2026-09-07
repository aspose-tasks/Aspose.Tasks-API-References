---
title: "UsageView.TopTimescaleTier"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti UsageView. Mendapatkan atau mengatur pengaturan tier skala waktu atas tampilan. TimescaleTier"
type: docs
weight: 80
url: /id/net/aspose.tasks/usageview/toptimescaletier/
---
## UsageView.TopTimescaleTier property

Mendapatkan atau mengatur pengaturan tier skala waktu atas tampilan. [`TimescaleTier`](../../../aspose.tasks.visualization/timescaletier/).

```csharp
public TimescaleTier TopTimescaleTier { get; set; }
```

## Contoh

Menunjukkan cara merender tampilan penggunaan tugas dengan pengaturan skala waktu yang didefinisikan dalam pengaturan tampilan.

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

// Definisikan SaveOptions dan tentukan bahwa pengaturan skala waktu TaskUsageView harus digunakan.
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.DefinedInView,
    PresentationFormat = PresentationFormat.TaskUsage
};

project.Save(OutDir + "TaskUsageView_CustomTimescale_out.pdf", options);
```

### Lihat Juga

* class [TimescaleTier](../../../aspose.tasks.visualization/timescaletier/)
* class [UsageView](../)
* namespace [Aspose.Tasks](../../usageview/)
* assembly [Aspose.Tasks](../../../)


