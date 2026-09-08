---
title: "GanttBarStyle.ShowForTaskUid"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство GanttBarStyle. Получает или задает уникальный идентификатор задачи, для которой применяется стиль. Применяется к стилизации полос в диаграмме Ганта, специфичной для задачи (см. CustomBarStyles)."
type: docs
weight: 210
url: /ru/net/aspose.tasks.visualization/ganttbarstyle/showfortaskuid/
---
## GanttBarStyle.ShowForTaskUid property

Получает и задает уникальный идентификатор задачи, для которой применяется стиль. Применяется к стилизации полос в диаграмме Ганта, специфичной для задачи (см. [`CustomBarStyles`](../../../aspose.tasks/ganttchartview/custombarstyles/)).

```csharp
public int? ShowForTaskUid { get; set; }
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


