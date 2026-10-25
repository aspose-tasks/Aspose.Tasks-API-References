---
title: "PageLegend.LegendOn"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية PageLegend. تحصل أو تضبط الصفحات التي تظهر فيها الأسطورة. يمكن أن تكون واحدة من قيم تعداد Legend."
type: docs
weight: 20
url: /ar/net/aspose.tasks.visualization/pagelegend/legendon/
---
## PageLegend.LegendOn property

تحصل أو تضبط الصفحات التي تظهر فيها الأسطورة. يمكن أن تكون واحدة من قيم تعداد [`Legend`](../../legend/).

```csharp
public Legend LegendOn { get; set; }
```

## الأمثلة

يعرض كيفية العمل مع معلومات أسطورة الصفحة.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

// دعنا نقرأ معلومات أسطورة الصفحة
var legend = project.DefaultView.PageInfo.Legend;

Console.WriteLine("Legend left text: {0} ", legend.LeftText);
Console.WriteLine("Legend left image: {0} ", legend.LeftImage);
Console.WriteLine("Legend center text: {0} ", legend.CenteredText);
Console.WriteLine("Legend center image: {0} ", legend.CenteredImage);
Console.WriteLine("Legend right text: {0} ", legend.RightText);
Console.WriteLine("Legend right image: {0} ", legend.RightImage);
Console.WriteLine("Legend On: {0} ", legend.LegendOn);
Console.WriteLine("Legend Width: {0} ", legend.Width);

// كما يُدعم تعديل الأسطورة
legend.LeftText = "New Left Text";

project.Save(OutDir + "WorkWithPageLegend_out.mpp", SaveFileFormat.Mpp);
```

### انظر أيضًا

* enum [Legend](../../legend/)
* class [PageLegend](../)
* namespace [Aspose.Tasks.Visualization](../../pagelegend/)
* assembly [Aspose.Tasks](../../../)


