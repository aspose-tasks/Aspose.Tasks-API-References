---
title: "الفئة PageSettings"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.Visualization.PageSettings. تمثل إعدادات الطباعة لصفحة من عرض المشروع"
type: docs
weight: 3240
url: /ar/net/aspose.tasks.visualization/pagesettings/
---
## PageSettings class

يمثل إعدادات الطباعة لصفحة من عرض المشروع.

```csharp
public class PageSettings
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [PageSettings](pagesettings/)() | ينشئ مثيلاً جديداً للفئة `PageSettings`. يمثل إعدادات الطباعة لصفحة من عرض المشروع. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [AdjustToPercentOfNormalSize](../../aspose.tasks.visualization/pagesettings/adjusttopercentofnormalsize/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب تعديل الطباعة إلى النسبة المئوية المحددة ([`PercentOfNormalSize`](./percentofnormalsize/)) من الحجم الطبيعي. |
| [FirstPageNumber](../../aspose.tasks.visualization/pagesettings/firstpagenumber/) { get; set; } | يحصل أو يعيّن رقم الصفحة الأولى للطباعة. |
| [IsPortrait](../../aspose.tasks.visualization/pagesettings/isportrait/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان اتجاه الصفحة عموديًا؛ تُعيد false إذا كان اتجاه الصفحة أفقيًا. |
| [PagesInHeight](../../aspose.tasks.visualization/pagesettings/pagesinheight/) { get; set; } | يحصل أو يعيّن عدد الصفحات في الارتفاع التي سيتم طباعتها. |
| [PagesInWidth](../../aspose.tasks.visualization/pagesettings/pagesinwidth/) { get; set; } | يحصل أو يعيّن عدد الصفحات في العرض التي سيتم طباعتها. |
| [PaperSize](../../aspose.tasks.visualization/pagesettings/papersize/) { get; set; } | يحصل أو يعيّن حجم الورق. يمكن أن يكون أحد قيم تعداد [`PrinterPaperSize`](../printerpapersize/). |
| [PaperSizeId](../../aspose.tasks.visualization/pagesettings/papersizeid/) { get; set; } | يحصل أو يعيّن عددًا صحيحًا يمثل أحد قيم PrinterPaperSize أو معرف حجم صفحة مخصص. يمكن استخدام هذه القيمة للحصول على حجم الورق من إعدادات نظام التشغيل. |
| [PercentOfNormalSize](../../aspose.tasks.visualization/pagesettings/percentofnormalsize/) { get; set; } | يحصل أو يعيّن نسبة مئوية من الحجم الطبيعي لتعديل الطباعة إليها. |

## الأمثلة

يعرض كيفية العمل مع &lt;see cref="Aspose.Tasks.Visualization.PageSettings" /&gt;.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// احصل على الإعدادات
var settings = project.DefaultView.PageInfo.PageSettings;
// دعنا نضبط بعض الخصائص
// عيّن قيمة تشير إلى ما إذا كان اتجاه الصفحة عموديًا؛ تُعيد false إذا كان اتجاه الصفحة أفقيًا.
settings.IsPortrait = true;
// عيّن عدد الصفحات في العرض التي سيتم طباعتها.
settings.PagesInWidth = 5;
// عيّن عدد الصفحات في الارتفاع التي سيتم طباعتها.
settings.PagesInHeight = 7;
// عيّن نسبة مئوية من الحجم الطبيعي لتعديل الطباعة إليها.
settings.PercentOfNormalSize = 200;
// عيّن حجم ورق. يمكن أن يكون أحد قيم تعداد <see cref="T:Aspose.Tasks.Visualization.PrinterPaperSize" />.
settings.PaperSize = PrinterPaperSize.PaperB4;
// عيّن رقم الصفحة الأولى للطباعة.
settings.FirstPageNumber = 3;

SimpleSaveOptions options = new MPPSaveOptions
{
    WriteViewData = true
};

project.Save(OutDir + "TestCanWritePageSettings.mpp", options);
```

### انظر أيضًا

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


