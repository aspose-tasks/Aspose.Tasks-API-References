---
title: "RecurringInterval.DailyDayNumber"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti RecurringInterval. Mendapatkan atau mengatur nomor hari harian"
type: docs
weight: 20
url: /id/net/aspose.tasks.visualization/recurringinterval/dailydaynumber/
---
## RecurringInterval.DailyDayNumber property

Mendapatkan atau mengatur nomor hari harian.

```csharp
public int DailyDayNumber { get; set; }
```

## Contoh

Menampilkan cara menambahkan interval berulang harian dari garis kemajuan.

```csharp
var project = new Project(DataDir + "Project2007.mpp");
project.Set(Prj.StatusDate, project.Get(Prj.StartDate));

var view = (GanttChartView)project.Views.ToList()[1];

view.ProgressLines.RecurringInterval = new RecurringInterval();
// atur nomor hari pola harian
view.ProgressLines.RecurringInterval.DailyDayNumber = 2;
// atur nilai yang menunjukkan apakah suatu hari adalah hari kerja untuk garis kemajuan harian.
view.ProgressLines.RecurringInterval.DailyWorkday = true;
```

### Lihat Juga

* class [RecurringInterval](../)
* namespace [Aspose.Tasks.Visualization](../../recurringinterval/)
* assembly [Aspose.Tasks](../../../)


