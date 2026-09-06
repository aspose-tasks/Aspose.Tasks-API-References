---
title: "الفئة Gridline"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.Visualization.Gridline. الخط الأفقي أو العمودي الذي يظهر في عرض المشروع"
type: docs
weight: 3100
url: /ar/net/aspose.tasks.visualization/gridline/
---
## Gridline class

الخط الأفقي أو العمودي الذي يظهر في عرض المشروع.

```csharp
public class Gridline
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [Gridline](gridline/)() | ينشئ مثيلاً جديداً من الفئة `Gridline`. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Color](../../aspose.tasks.visualization/gridline/color/) { get; set; } | يحصل أو يضبط الـ[`Color`](./color/) لخط الشبكة. |
| [GridlineType](../../aspose.tasks.visualization/gridline/gridlinetype/) { get; set; } | يحصل أو يضبط نوع خط الشبكة ([`GridlineType`](./gridlinetype/)). |
| [Pattern](../../aspose.tasks.visualization/gridline/pattern/) { get; set; } | يحصل أو يضبط الـ[`LinePattern`](../linepattern/) لخط الشبكة. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| override [Equals](../../aspose.tasks.visualization/gridline/equals/)(object) | يرجع علامة تشير إلى ما إذا كانت هذه المثيلة مساوية للعنصر المحدد. |
| override [GetHashCode](../../aspose.tasks.visualization/gridline/gethashcode/)() | يرجع قيمة رمز تجزئة للمثيل من الفئة `Gridline`. |

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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


