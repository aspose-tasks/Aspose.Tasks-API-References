---
title: "UsageView.DisplayShortDetailHeaderNames"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "UsageView property. Mendapatkan atau mengatur nilai yang menunjukkan apakah menampilkan nama header detail singkat atau tidak"
type: docs
weight: 40
url: /id/net/aspose.tasks/usageview/displayshortdetailheadernames/
---
## UsageView.DisplayShortDetailHeaderNames property

Mendapatkan atau mengatur nilai yang menunjukkan apakah menampilkan nama header detail singkat atau tidak.

```csharp
public bool DisplayShortDetailHeaderNames { get; set; }
```

## Contoh

Menampilkan cara merender tampilan penggunaan tugas dengan detail.

```csharp
var project = new Project(DataDir + "TaskUsageViewWithDetails.mpp");

// dapatkan tampilan
UsageView view = (TaskUsageView)project.DefaultView;

// kolom header detail tidak akan ditampilkan
view.DisplayDetailsHeaderColumn = false;
view.RepeatDetailsHeaderOnAllRows = false;
view.DisplayShortDetailHeaderNames = false;
view.AlignDetailsData = HorizontalStringAlignment.Near;
project.Save(OutDir + "task usage1_out.pdf", SaveFileFormat.Pdf);

// tampilkan kolom header detail
view.DisplayDetailsHeaderColumn = true;

// ulangi header detail pada semua baris penugasan
view.RepeatDetailsHeaderOnAllRows = true;
view.AlignDetailsData = HorizontalStringAlignment.Far;
project.Save(OutDir + "task usage2_out.pdf", SaveFileFormat.Pdf);
```

### Lihat Juga

* class [UsageView](../)
* namespace [Aspose.Tasks](../../usageview/)
* assembly [Aspose.Tasks](../../../)


