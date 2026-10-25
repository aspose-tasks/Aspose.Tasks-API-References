---
title: "Gridline.GridlineType"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية Gridline. تحصل أو تضبط نوع خط الشبكة GridlineType."
type: docs
weight: 30
url: /ar/net/aspose.tasks.visualization/gridline/gridlinetype/
---
## Gridline.GridlineType property

تحصل أو تضبط نوع خط الشبكة (`GridlineType`).

```csharp
public GridlineType GridlineType { get; set; }
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

* enum [GridlineType](../../gridlinetype/)
* class [Gridline](../)
* namespace [Aspose.Tasks.Visualization](../../gridline/)
* assembly [Aspose.Tasks](../../../)


