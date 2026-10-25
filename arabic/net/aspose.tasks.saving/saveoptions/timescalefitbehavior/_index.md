---
title: "SaveOptions.TimescaleFitBehavior"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية SaveOptions. يحصل أو يضبط سلوكًا يحدد كيفية محاذاة الطرف الأيمن للمقياس الزمني مع نهاية الصفحة"
type: docs
weight: 210
url: /ar/net/aspose.tasks.saving/saveoptions/timescalefitbehavior/
---
## SaveOptions.TimescaleFitBehavior property

يحصل أو يعيّن سلوكًا يحدد كيفية محاذاة الطرف الأيمن للمقياس الزمني مع نهاية الصفحة.

```csharp
public TimescaleFitBehavior TimescaleFitBehavior { get; set; }
```

## الأمثلة

يوضح كيفية استخدام TimescaleFitBehavior لجعل مقياس وقت مخطط جانت يتلاءم مع نهاية الصفحة الأخيرة.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var view = project.DefaultView as GanttChartView;

PdfSaveOptions saveOptions = new PdfSaveOptions();
saveOptions.PageSize = PageSize.A4;
saveOptions.StartDate = project.StartDate;
saveOptions.EndDate = project.FinishDate;
saveOptions.ViewSettings = view;
saveOptions.TimescaleFitBehavior = TimescaleFitBehavior.ScaleToEndOfPage;

project.Save(OutDir + "WorkWithPageSizeDefinedInView_out.pdf", saveOptions);
```

### انظر أيضًا

* enum [TimescaleFitBehavior](../../../aspose.tasks.visualization/timescalefitbehavior/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


