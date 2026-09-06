---
title: "الفئة PageViewSettings"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "فئة Aspose.Tasks.Visualization.PageViewSettings. تمثل إعدادات الطباعة لعرض المشروع"
type: docs
weight: 3260
url: /ar/net/aspose.tasks.visualization/pageviewsettings/
---
## PageViewSettings class

يمثل إعدادات الطباعة لعرض المشروع.

```csharp
public class PageViewSettings
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [PageViewSettings](pageviewsettings/)() | المنشئ الافتراضي. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [FirstColumnsCount](../../aspose.tasks.visualization/pageviewsettings/firstcolumnscount/) { get; set; } | يحصل أو يعيّن عدد الأعمدة الأولى التي تُطبع في جميع الصفحات. |
| [FitTimescaleToEndOfPage](../../aspose.tasks.visualization/pageviewsettings/fittimescaletoendofpage/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب ملاءمة مقياس الوقت إلى نهاية الصفحة عند الطباعة. |
| [PrintAllSheetColumns](../../aspose.tasks.visualization/pageviewsettings/printallsheetcolumns/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب طباعة جميع أعمدة الورقة في العرض. |
| [PrintBlankPages](../../aspose.tasks.visualization/pageviewsettings/printblankpages/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب طباعة الصفحات الفارغة للعرض. |
| [PrintFirstColumnsCountOnAllPages](../../aspose.tasks.visualization/pageviewsettings/printfirstcolumnscountonallpages/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب طباعة عدد محدد من الأعمدة الأولى في جميع الصفحات. |
| [PrintNotes](../../aspose.tasks.visualization/pageviewsettings/printnotes/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب طباعة الملاحظات. |

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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


