---
title: "PageViewSettings.PrintFirstColumnsCountOnAllPages"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية PageViewSettings. يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب طباعة عدد محدد من الأعمدة الأولى على جميع الصفحات"
type: docs
weight: 60
url: /ar/net/aspose.tasks.visualization/pageviewsettings/printfirstcolumnscountonallpages/
---
## PageViewSettings.PrintFirstColumnsCountOnAllPages property

يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب طباعة عدد محدد من الأعمدة الأولى في جميع الصفحات.

```csharp
public bool PrintFirstColumnsCountOnAllPages { get; set; }
```

## الأمثلة

يظهر كيفية طباعة ملاحظات المهمة والموارد والتعيين في صفحة منفصلة.

```csharp
var project = new Project(DataDir + "Input.mpp");

// تعيين عدد الأعمدة الأولى التي سيتم طباعتها على جميع الصفحات
project.DefaultView.PageInfo.PageViewSettings.FirstColumnsCount = 2;

// عيّن قيمة تشير إلى ما إذا كان يجب طباعة الملاحظات.
project.DefaultView.PageInfo.PageViewSettings.PrintNotes = true;

// عيّن قيمة تشير إلى ما إذا كان يجب ملاءمة مقياس الوقت إلى نهاية الصفحة عند الطباعة.
project.DefaultView.PageInfo.PageViewSettings.FitTimescaleToEndOfPage = true;

// عيّن قيمة تشير إلى ما إذا كان يجب طباعة جميع أعمدة الورقة في العرض
project.DefaultView.PageInfo.PageViewSettings.PrintAllSheetColumns = true;

// عيّن قيمة تشير إلى ما إذا كان يجب طباعة الصفحات الفارغة للعرض
project.DefaultView.PageInfo.PageViewSettings.PrintBlankPages = false;

// تعيين قيمة تشير إلى ما إذا كان يجب طباعة عدد محدد من الأعمدة الأولى على جميع الصفحات
project.DefaultView.PageInfo.PageViewSettings.PrintFirstColumnsCountOnAllPages = true;

project.Save(OutDir + "ProjectWithComments_out.pdf", SaveFileFormat.Pdf);
```

### انظر أيضًا

* class [PageViewSettings](../)
* namespace [Aspose.Tasks.Visualization](../../pageviewsettings/)
* assembly [Aspose.Tasks](../../../)


