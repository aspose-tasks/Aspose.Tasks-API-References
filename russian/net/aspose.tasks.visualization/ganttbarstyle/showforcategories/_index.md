---
title: "GanttBarStyle.ShowForCategories"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство GanttBarStyle. Получает или задает категории задач, для которых применяется стиль. Применяется к родительским или общим стилям полос в диаграмме Ганта, см. BarStyles"
type: docs
weight: 200
url: /ru/net/aspose.tasks.visualization/ganttbarstyle/showforcategories/
---
## GanttBarStyle.ShowForCategories property

Получает или задает категории задач, для которых применяется стиль. Применяется к родительским (или общим) стилям полос в диаграмме Ганта (см. [`BarStyles`](../../../aspose.tasks/ganttchartview/barstyles/)).

```csharp
public IList<GanttBarShowFor> ShowForCategories { get; set; }
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

* enum [GanttBarShowFor](../../ganttbarshowfor/)
* class [GanttBarStyle](../)
* namespace [Aspose.Tasks.Visualization](../../ganttbarstyle/)
* assembly [Aspose.Tasks](../../../)


