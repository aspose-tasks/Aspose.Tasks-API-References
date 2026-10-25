---
title: "GanttBarStyle.ShowForTaskUid"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "GanttBarStyle özelliği. Stilinin uygulandığı görevin benzersiz kimliğini alır veya ayarlar. Gantt şemasındaki çubukların görev‑spesifik stillerine uygulanabilir, bkz. CustomBarStyles"
type: docs
weight: 210
url: /tr/net/aspose.tasks.visualization/ganttbarstyle/showfortaskuid/
---
## GanttBarStyle.ShowForTaskUid property

Stilinin uygulandığı görevin benzersiz kimliğini alır veya ayarlar. Gantt şemasındaki çubukların görev‑spesifik stillerine uygulanabilir (bkz. [`CustomBarStyles`](../../../aspose.tasks/ganttchartview/custombarstyles/)).

```csharp
public int? ShowForTaskUid { get; set; }
```

## Örnekler

ShowFor kategorilerinin nasıl kullanılacağını gösterir.

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

// projeyle çalış...
```

### Ayrıca Bakınız

* class [GanttBarStyle](../)
* namespace [Aspose.Tasks.Visualization](../../ganttbarstyle/)
* assembly [Aspose.Tasks](../../../)


