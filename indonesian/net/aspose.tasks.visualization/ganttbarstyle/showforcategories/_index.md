---
title: "GanttBarStyle.ShowForCategories"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti GanttBarStyle. Mendapatkan atau mengatur kategori tugas yang gaya diterapkan. Berlaku untuk gaya induk atau umum batang pada diagram Gantt, lihat BarStyles"
type: docs
weight: 200
url: /id/net/aspose.tasks.visualization/ganttbarstyle/showforcategories/
---
## GanttBarStyle.ShowForCategories property

Mendapatkan atau mengatur kategori tugas yang gaya diterapkan. Berlaku untuk gaya induk (atau umum) batang pada diagram Gantt (lihat [`BarStyles`](../../../aspose.tasks/ganttchartview/barstyles/)).

```csharp
public IList<GanttBarShowFor> ShowForCategories { get; set; }
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

* enum [GanttBarShowFor](../../ganttbarshowfor/)
* class [GanttBarStyle](../)
* namespace [Aspose.Tasks.Visualization](../../ganttbarstyle/)
* assembly [Aspose.Tasks](../../../)


