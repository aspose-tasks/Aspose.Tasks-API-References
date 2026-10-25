---
title: "GanttBarStyle.ShowForTaskUid"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti GanttBarStyle. Mendapatkan atau mengatur Id Unik dari tugas yang gaya diterapkan. Berlaku untuk gaya khusus batang pada diagram Gantt, lihat CustomBarStyles."
type: docs
weight: 210
url: /id/net/aspose.tasks.visualization/ganttbarstyle/showfortaskuid/
---
## GanttBarStyle.ShowForTaskUid property

Mendapatkan dan mengatur Id Unik dari tugas yang gaya diterapkan. Berlaku untuk gaya khusus batang pada diagram Gantt (lihat [`CustomBarStyles`](../../../aspose.tasks/ganttchartview/custombarstyles/)).

```csharp
public int? ShowForTaskUid { get; set; }
```

## Contoh

Menampilkan cara menggunakan kategori ShowFor.

```csharp
var project = new Project(DataDir + "Project2.mpp");
var view = (GanttChartView)project.DefaultView;

var barStyle = this.GetCustomBarStyle();
barStyle.ShowForTaskUid = null;

var showForCategories = new[]
{
    GanttBarShowFor.Active,
    GanttBarShowFor.NotSummary,
    GanttBarShowFor.Milestone,
    GanttBarShowFor.Finished
};

barStyle.ShowForCategories = new List<GanttBarShowFor>(showForCategories);
barStyle.Name = "My common style";
view.BarStyles.Add(barStyle);

// bekerja dengan proyek...
```

### Lihat Juga

* class [GanttBarStyle](../)
* namespace [Aspose.Tasks.Visualization](../../ganttbarstyle/)
* assembly [Aspose.Tasks](../../../)


