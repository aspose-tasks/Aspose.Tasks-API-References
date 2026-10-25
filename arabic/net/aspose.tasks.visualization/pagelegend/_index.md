---
title: "الفئة PageLegend"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.Visualization.PageLegend. تمثل أسطورة الصفحة التي تُستخدم لطباعة المشروع."
type: docs
weight: 3210
url: /ar/net/aspose.tasks.visualization/pagelegend/
---
## PageLegend class

يمثل أسطورة الصفحة التي تُستخدم لطباعة المشروع.

```csharp
public class PageLegend : HeaderFooterInfo
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [PageLegend](pagelegend/)() | المنشئ الافتراضي. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [CenteredImage](../../aspose.tasks.visualization/headerfooterinfo/centeredimage/) { get; set; } | يحصل أو يعيّن الصورة المركزية التي ستُعرض في العنصر الأب. |
| [CenteredImageSize](../../aspose.tasks.visualization/headerfooterinfo/centeredimagesize/) { get; set; } | يحصل أو يعيّن الحجم المعروض للصورة المركزية. |
| [CenteredText](../../aspose.tasks.visualization/headerfooterinfo/centeredtext/) { get; set; } | يحصل أو يعيّن النص المركزي لعرضه في العنصر الأب. |
| [LeftImage](../../aspose.tasks.visualization/headerfooterinfo/leftimage/) { get; set; } | يحصل أو يعيّن الصورة المحاذاة إلى اليسار التي تُعرض في العنصر الأب. |
| [LeftImageSize](../../aspose.tasks.visualization/headerfooterinfo/leftimagesize/) { get; set; } | يحصل أو يعيّن حجم الصورة اليسرى المعروض. |
| [LeftText](../../aspose.tasks.visualization/headerfooterinfo/lefttext/) { get; set; } | يحصل أو يعيّن النص المحاذى إلى اليسار لعرضه في العنصر الأب. |
| [LegendOn](../../aspose.tasks.visualization/pagelegend/legendon/) { get; set; } | يحصل أو يضبط الصفحات التي تظهر فيها الأسطورة. يمكن أن تكون إحدى قيم تعداد [`Legend`](../legend/). |
| [RightImage](../../aspose.tasks.visualization/headerfooterinfo/rightimage/) { get; set; } | يحصل أو يعيّن الصورة المحاذاة إلى اليمين لتُعرض في العنصر الأب. |
| [RightImageSize](../../aspose.tasks.visualization/headerfooterinfo/rightimagesize/) { get; set; } | يحصل أو يعيّن حجم الصورة اليمنى المعروض. |
| [RightText](../../aspose.tasks.visualization/headerfooterinfo/righttext/) { get; set; } | يحصل أو يعيّن النص المحاذى إلى اليمين لعرضه في العنصر الأب. |
| [Width](../../aspose.tasks.visualization/pagelegend/width/) { get; set; } | يحصل أو يضبط عرض الجزء الأيسر (الذي يحتوي على اسم المشروع وتاريخه افتراضياً) من الأسطورة بالسنتيمترات. |

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

* class [HeaderFooterInfo](../headerfooterinfo/)
* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


