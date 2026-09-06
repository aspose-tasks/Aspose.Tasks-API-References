---
title: "PageLegend.RightImage"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية PageLegend. يحصل أو يضبط الصورة المحاذاة إلى اليمين لتظهر في وسيلة إيضاح الصفحة"
type: docs
weight: 70
url: /ar/net/aspose.tasks.visualization/pagelegend/rightimage/
---
## PageLegend.RightImage property

يحصل أو يضبط الصورة المحاذاة إلى اليمين لتظهر في وسيلة إيضاح الصفحة.

```csharp
public Image RightImage { get; set; }
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

* class [PageLegend](../)
* namespace [Aspose.Tasks.Visualization](../../pagelegend/)
* assembly [Aspose.Tasks](../../../)


