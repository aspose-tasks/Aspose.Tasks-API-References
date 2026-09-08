---
title: "GanttBarStyle.Name"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство GanttBarStyle. Получает или задает имя стиля."
type: docs
weight: 150
url: /ru/net/aspose.tasks.visualization/ganttbarstyle/name/
---
## GanttBarStyle.Name property

Получает или задает название стиля.

```csharp
public string Name { get; set; }
```

## Примеры

Показывает, как использовать категории ShowFor.

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

// работать с проектом...
```

### См. также

* class [GanttBarStyle](../)
* namespace [Aspose.Tasks.Visualization](../../ganttbarstyle/)
* assembly [Aspose.Tasks](../../../)


