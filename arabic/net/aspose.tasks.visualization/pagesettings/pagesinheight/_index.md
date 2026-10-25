---
title: "PageSettings.PagesInHeight"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية PageSettings. تحصل أو تضبط عدد الصفحات في الارتفاع التي سيتم طباعتها"
type: docs
weight: 50
url: /ar/net/aspose.tasks.visualization/pagesettings/pagesinheight/
---
## PageSettings.PagesInHeight property

يحصل أو يعيّن عدد الصفحات في الارتفاع التي سيتم طباعتها.

```csharp
public int PagesInHeight { get; set; }
```

## الأمثلة

يعرض كيفية عرض المشهد باستخدام خيار 'Fit X to Y pages'.

```csharp
var project = new Project(DataDir + "TaskUsageView.mpp");

var view = project.Views.First(v => v.Screen == ViewScreen.TaskUsage);

view.PageInfo.PageSettings.AdjustToPercentOfNormalSize = false;
// حدد أن المشهد يجب أن يُعرض في صفحتين أو أقل في الارتفاع
view.PageInfo.PageSettings.PagesInHeight = 2;
// حدد أن المشهد يجب أن يُعرض في صفحة واحدة في العرض
view.PageInfo.PageSettings.PagesInWidth = 1;

PdfSaveOptions saveOptions = new PdfSaveOptions()
{
    ViewSettings = view,
    Timescale = Timescale.DefinedInView,
    StartDate =  new DateTime(2000, 04, 1),
    EndDate = new DateTime(2000, 12, 31)
};

project.Save(OutDir + "PrintViewWithFitToPages_out.pdf", saveOptions);
```

### انظر أيضًا

* class [PageSettings](../)
* namespace [Aspose.Tasks.Visualization](../../pagesettings/)
* assembly [Aspose.Tasks](../../../)


