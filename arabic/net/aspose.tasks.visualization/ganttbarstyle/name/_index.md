---
title: "GanttBarStyle.Name"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية GanttBarStyle. يحصل أو يضبط اسم النمط"
type: docs
weight: 150
url: /ar/net/aspose.tasks.visualization/ganttbarstyle/name/
---
## GanttBarStyle.Name property

يحصل أو يعيّن اسم النمط.

```csharp
public string Name { get; set; }
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

* class [GanttBarStyle](../)
* namespace [Aspose.Tasks.Visualization](../../ganttbarstyle/)
* assembly [Aspose.Tasks](../../../)


