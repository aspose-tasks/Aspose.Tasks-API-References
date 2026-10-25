---
title: "الفئة PageInfo"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.Visualization.PageInfo. تمثل بيانات إعداد الصفحة الموجودة في تنسيق ملف MPP وتُستخدم للطباعة."
type: docs
weight: 3200
url: /ar/net/aspose.tasks.visualization/pageinfo/
---
## PageInfo class

يمثل بيانات إعداد الصفحة الموجودة في تنسيق ملف MPP والمستخدمة للطباعة.

```csharp
public class PageInfo
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [PageInfo](pageinfo/)() | ينشئ مثيلاً جديداً من الفئة `PageInfo`. تمثل بيانات إعداد الصفحة الموجودة في تنسيق ملف MPP وتُستخدم للطباعة. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Footer](../../aspose.tasks.visualization/pageinfo/footer/) { get; set; } | يحصل أو يضبط مثيلاً من الفئة [`HeaderFooterInfo`](../headerfooterinfo/) التي تمثل بيانات تذييل. |
| [Header](../../aspose.tasks.visualization/pageinfo/header/) { get; set; } | يحصل أو يضبط مثيلاً من الفئة [`HeaderFooterInfo`](../headerfooterinfo/) التي تمثل بيانات رأس. |
| [Legend](../../aspose.tasks.visualization/pageinfo/legend/) { get; set; } | يحصل أو يضبط مثيلاً من الفئة [`PageLegend`](../pagelegend/) التي تحدد خيارات عرض أسطورة الصفحة. |
| [Margins](../../aspose.tasks.visualization/pageinfo/margins/) { get; } | يحصل على مثيل من الفئة [`PageMargins`](../pagemargins/) التي تحدد هوامش الصفحة. |
| [Name](../../aspose.tasks.visualization/pageinfo/name/) { get; } | يحصل على اسم العرض الذي تُستخدم له بيانات الإعداد. |
| [PageSettings](../../aspose.tasks.visualization/pageinfo/pagesettings/) { get; } | يحصل على مثيل من الفئة [`PageSettings`](./pagesettings/) التي تحدد إعدادات طباعة الصفحة. |
| [PageViewSettings](../../aspose.tasks.visualization/pageinfo/pageviewsettings/) { get; } | يحصل على مثيل من الفئة [`PageViewSettings`](./pageviewsettings/) التي تحدد إعدادات طباعة عرض الصفحة. |

## الأمثلة

يعرض كيفية العمل مع معلومات الصفحة في عرض MS Project.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// دعنا نعدّل العرض الافتراضي.
var info = project.DefaultView.PageInfo;

Console.WriteLine("Modify Page Info: " + info.Name);

// دعنا نعدّل الهوامش.
info.Margins.Left = 10d;
info.Margins.Top = 10d;
info.Margins.Right = 10d;
info.Margins.Bottom = 10d;

// دعنا نُعدّل إعدادات الصفحة
info.PageSettings.IsPortrait = true;
info.PageSettings.PaperSize = PrinterPaperSize.PaperA4;

// دعنا نُعدّل إعدادات عرض الصفحة
// عيّن قيمة تشير إلى ما إذا كان يجب طباعة الملاحظات.
info.PageViewSettings.PrintNotes = true;

var header = new HeaderFooterInfo
{
    LeftText = "Left header text",
    CenteredText = "Centered header text",
    RightText = "Right header text"
};
var legend = new PageLegend
{
    LeftText =  "Left legend text",
    CenteredText = "Centered legend text",
    RightText = "Right legend text"
};
var footer = new HeaderFooterInfo
{
    LeftText = "Left footer text",
    CenteredText = "Centered footer text",
    RightText = "Right footer text"
};

info.Header = header;
info.Legend = legend;
info.Footer = footer;

// العمل مع المشروع...
```

### انظر أيضًا

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


