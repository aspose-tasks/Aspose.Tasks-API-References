---
title: "UsageView.RepeatDetailsHeaderOnAllRows"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti UsageView. Mendapatkan atau mengatur nilai yang menunjukkan apakah mengulangi header detail pada semua baris penugasan atau tidak"
type: docs
weight: 60
url: /id/net/aspose.tasks/usageview/repeatdetailsheaderonallrows/
---
## UsageView.RepeatDetailsHeaderOnAllRows property

Mendapatkan atau mengatur nilai yang menunjukkan apakah mengulangi header detail pada semua baris penugasan atau tidak.

```csharp
public bool RepeatDetailsHeaderOnAllRows { get; set; }
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


