---
title: "GanttBarStyle.Name"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "GanttBarStyle özelliği. Stil adını alır veya ayarlar"
type: docs
weight: 150
url: /tr/net/aspose.tasks.visualization/ganttbarstyle/name/
---
## GanttBarStyle.Name property

Stil adını alır veya ayarlar.

```csharp
public string Name { get; set; }
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


