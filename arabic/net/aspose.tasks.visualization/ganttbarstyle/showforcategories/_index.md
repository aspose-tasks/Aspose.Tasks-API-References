---
title: "GanttBarStyle.ShowForCategories"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية GanttBarStyle. يحصل أو يعيّن فئات المهام التي يُطبق عليها النمط. يُطبق على الأنماط الأب أو المشتركة للأعمدة في مخطط Gantt راجع BarStyles"
type: docs
weight: 200
url: /ar/net/aspose.tasks.visualization/ganttbarstyle/showforcategories/
---
## GanttBarStyle.ShowForCategories property

يحصل أو يعيّن فئات المهام التي يُطبق عليها النمط. يُطبق على الأنماط الأب (أو المشتركة) للأعمدة في مخطط Gantt (انظر [`BarStyles`](../../../aspose.tasks/ganttchartview/barstyles/)).

```csharp
public IList<GanttBarShowFor> ShowForCategories { get; set; }
```

## الأمثلة

يعرض كيفية استخدام فئات ShowFor.

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

// العمل مع المشروع...
```

### انظر أيضًا

* enum [GanttBarShowFor](../../ganttbarshowfor/)
* class [GanttBarStyle](../)
* namespace [Aspose.Tasks.Visualization](../../ganttbarstyle/)
* assembly [Aspose.Tasks](../../../)


