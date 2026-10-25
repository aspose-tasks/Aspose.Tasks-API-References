---
title: "GanttBarStyle.Name"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti GanttBarStyle. Mendapatkan atau mengatur nama gaya."
type: docs
weight: 150
url: /id/net/aspose.tasks.visualization/ganttbarstyle/name/
---
## GanttBarStyle.Name property

Mendapatkan atau mengatur nama gaya.

```csharp
public string Name { get; set; }
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


