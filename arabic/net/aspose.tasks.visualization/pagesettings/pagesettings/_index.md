---
title: "PageSettings.PageSettings"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "منشئ PageSettings. يهيئ نسخة جديدة من فئة PageSettings. يمثل إعدادات الطباعة لصفحة من عرض المشروع."
type: docs
weight: 10
url: /ar/net/aspose.tasks.visualization/pagesettings/pagesettings/
---
## PageSettings constructor

يهيئ نسخة جديدة من الفئة [`PageSettings`](../). يمثل إعدادات الطباعة لصفحة من عرض المشروع.

```csharp
public PageSettings()
```

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

* class [PageSettings](../)
* namespace [Aspose.Tasks.Visualization](../../pagesettings/)
* assembly [Aspose.Tasks](../../../)


