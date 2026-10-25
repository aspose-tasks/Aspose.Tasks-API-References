---
title: "SaveOptions.IsPortrait"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية SaveOptions. يحصل أو يحدد قيمة تشير إلى ما إذا كان اتجاه الصفحة عموديًا، يرجع false إذا كان اتجاه الصفحة أفقيًا"
type: docs
weight: 70
url: /ar/net/aspose.tasks.saving/saveoptions/isportrait/
---
## SaveOptions.IsPortrait property

يحصل أو يعيّن قيمة تشير إلى ما إذا كان اتجاه الصفحة عموديًا؛ تُعيد false إذا كان اتجاه الصفحة أفقيًا.

```csharp
public bool IsPortrait { get; set; }
```

## ملاحظات

غير قابل للتطبيق عندما SaveOptions.PageSize == Visualization.PageSize.DefinedInView. في هذه الحالة يتم استخدام View.PageInfo.PageSettings.IsPortrait بدلاً من ذلك. غير قابل للتطبيق عندما يتم تعيين SaveOptions.CustomPageSize.

## الأمثلة

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

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


