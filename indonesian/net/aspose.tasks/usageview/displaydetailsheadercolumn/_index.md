---
title: "UsageView.DisplayDetailsHeaderColumn"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti UsageView. Mendapatkan atau mengatur nilai yang menunjukkan apakah menampilkan kolom header detail dalam tampilan atau tidak"
type: docs
weight: 30
url: /id/net/aspose.tasks/usageview/displaydetailsheadercolumn/
---
## UsageView.DisplayDetailsHeaderColumn property

Mendapatkan atau mengatur nilai yang menunjukkan apakah menampilkan kolom header detail dalam tampilan atau tidak.

```csharp
public bool DisplayDetailsHeaderColumn { get; set; }
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


