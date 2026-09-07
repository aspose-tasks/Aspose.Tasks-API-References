---
title: "GanttChartView.AutoFilters"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti GanttChartView. Mendapatkan daftar filter otomatis dari tampilan Gantt Chart"
type: docs
weight: 20
url: /id/net/aspose.tasks/ganttchartview/autofilters/
---
## GanttChartView.AutoFilters property

Mendapatkan daftar filter otomatis dari tampilan Gantt Chart.

```csharp
public FilterCollection AutoFilters { get; }
```

## Contoh

Menampilkan cara membaca filter otomatis dari tampilan diagram Gantt.

```csharp
var project = new Project(DataDir + "AutoFilterOnFinishColumn.mpp");
project.Set(Prj.StatusDate, project.Get(Prj.StartDate));

var view = (GanttChartView)project.Views.First(v => v.Screen == ViewScreen.Gantt);

// mengiterasi filter otomatis dari tampilan diagram Gantt
foreach (var filter in view.AutoFilters)
{
    Console.WriteLine("Criteria: " + filter.Criteria);

    Console.WriteLine("Criteria field: " + filter.Criteria.Field);
    Console.WriteLine("Criteria test condition: " + filter.Criteria.Test);
    Console.WriteLine("Criteria values: " + string.Join(", ", filter.Criteria.Values.Where(c => c != null)));
    Console.WriteLine();
}

// bekerja dengan proyek...
```

### Lihat Juga

* class [FilterCollection](../../filtercollection/)
* class [GanttChartView](../)
* namespace [Aspose.Tasks](../../ganttchartview/)
* assembly [Aspose.Tasks](../../../)


