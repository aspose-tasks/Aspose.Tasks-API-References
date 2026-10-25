---
title: "PageSettings.IsPortrait"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية PageSettings. تحصل أو تضبط قيمة تشير إلى ما إذا كان اتجاه الصفحة عموديًا وتعيد false إذا كان اتجاه الصفحة أفقيًا"
type: docs
weight: 40
url: /ar/net/aspose.tasks.visualization/pagesettings/isportrait/
---
## PageSettings.IsPortrait property

يحصل أو يعيّن قيمة تشير إلى ما إذا كان اتجاه الصفحة عموديًا؛ تُعيد false إذا كان اتجاه الصفحة أفقيًا.

```csharp
public bool IsPortrait { get; set; }
```

## ملاحظات

يطبق أثناء العرض عندما SaveOptions.PageSize == Visualization.PageSize.DefinedInView.

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

يوضح كيفية تحديد حجم الصفحة والاتجاه باستخدام إعدادات View أو باستخدام SaveOptions.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var view = project.Views.First(v => v.Screen == ViewScreen.Gantt);

PdfSaveOptions saveOptions = new PdfSaveOptions();
saveOptions.Timescale = Timescale.DefinedInView;
saveOptions.StartDate = new DateTime(2012, 12, 22);
saveOptions.EndDate = new DateTime(2013, 05, 10);
saveOptions.ViewSettings = view;

saveOptions.PageSize = PageSize.DefinedInView;

// في هذه الحالة يتم تطبيق حجم الصفحة والاتجاه من خصائص view.PageInfo.PageSettings.PaperSize و view.PageInfo.PageSettings.IsPortrait.
project.Save(OutDir + "WorkWithIsPortrait_out1.pdf", saveOptions);

saveOptions.PageSize = PageSize.A4;
saveOptions.IsPortrait = true;

// في هذه الحالة يتم تطبيق حجم الصفحة والاتجاه من خصائص SaveOptions.
project.Save(OutDir + "WorkWithIsPortrait_out2.pdf", saveOptions);

saveOptions.CustomPageSize = new SizeF(400, 600);

// في هذه الحالة يتم تطبيق حجم الصفحة من SaveOptions.CustomPageSize. لا يتم أخذ خاصية IsPortrait في الاعتبار.
project.Save(OutDir + "WorkWithIsPortrait_out3.pdf", saveOptions);
```

### انظر أيضًا

* class [PageSettings](../)
* namespace [Aspose.Tasks.Visualization](../../pagesettings/)
* assembly [Aspose.Tasks](../../../)


