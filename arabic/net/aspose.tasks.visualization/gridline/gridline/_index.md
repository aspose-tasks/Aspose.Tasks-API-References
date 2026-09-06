---
title: "Gridline.Gridline"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "منشئ Gridline. يهيئ مثيلاً جديداً من فئة Gridline."
type: docs
weight: 10
url: /ar/net/aspose.tasks.visualization/gridline/gridline/
---
## Gridline constructor

يهيئ مثيلاً جديداً من فئة [`Gridline`](../).

```csharp
public Gridline()
```

## الأمثلة

يوضح كيفية العمل مع خطوط الشبكة أثناء الحفظ بصيغ بصرية.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
var options = new ImageSaveOptions(SaveFileFormat.Png);

var gridline = new Gridline
{
    // تعيين نوع خط الشبكة (<see cref=\"P:Aspose.Tasks.Visualization.Gridline.GridlineType\" />).
    GridlineType = GridlineType.GanttRow, 
    // تعيين <see cref=\"T:Aspose.Tasks.Visualization.LinePattern\" /> لخط الشبكة
    Pattern = LinePattern.Dashed
};

options.Gridlines = new List<Gridline>();
options.Gridlines.Add(gridline);

project.Save(OutDir + "PrintProjectPagesToSeparateFiles_out.png", options);
```

### انظر أيضًا

* class [Gridline](../)
* namespace [Aspose.Tasks.Visualization](../../gridline/)
* assembly [Aspose.Tasks](../../../)


