---
title: "GanttBarStyle.ShowForCategories"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "GanttBarStyle özelliği. Stilinin uygulandığı görev kategorilerini alır veya ayarlar. Gantt grafiğindeki çubukların üst veya ortak stillerine uygulanabilir, bkz. BarStyles"
type: docs
weight: 200
url: /tr/net/aspose.tasks.visualization/ganttbarstyle/showforcategories/
---
## GanttBarStyle.ShowForCategories property

Stilin uygulandığı görev kategorilerini alır veya ayarlar. Gantt grafiğindeki çubukların üst (veya ortak) stillerine uygulanabilir (bkz. [`BarStyles`](../../../aspose.tasks/ganttchartview/barstyles/)).

```csharp
public IList<GanttBarShowFor> ShowForCategories { get; set; }
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

* enum [GanttBarShowFor](../../ganttbarshowfor/)
* class [GanttBarStyle](../)
* namespace [Aspose.Tasks.Visualization](../../ganttbarstyle/)
* assembly [Aspose.Tasks](../../../)


