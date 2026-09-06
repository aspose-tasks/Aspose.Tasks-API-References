---
title: "PageSettings.PercentOfNormalSize"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية PageSettings. تحصل أو تضبط نسبة مئوية من الحجم الطبيعي لضبط الطباعة إلى"
type: docs
weight: 90
url: /ar/net/aspose.tasks.visualization/pagesettings/percentofnormalsize/
---
## PageSettings.PercentOfNormalSize property

يحصل أو يعيّن نسبة مئوية من الحجم الطبيعي لتعديل الطباعة إليها.

```csharp
public int PercentOfNormalSize { get; set; }
```

## الأمثلة

يعرض كيفية عرض المشهد باستخدام عامل المقياس المحدد.

```csharp
var project = new Project(DataDir + "Input.mpp");

var view = project.Views.First(v => v.Screen == ViewScreen.Gantt);

// اضبط قيمة تشير إلى أن المشهد يجب أن يُقاس باستخدام عامل المقياس المحدد
view.PageInfo.PageSettings.AdjustToPercentOfNormalSize = true;
// حدد عامل المقياس
view.PageInfo.PageSettings.PercentOfNormalSize = 33;

PdfSaveOptions saveOptions = new PdfSaveOptions()
{
    ViewSettings = view,
    Timescale = Timescale.DefinedInView
};

project.Save(OutDir + "PrintViewWithSpecifiedScaleFactor_out.pdf", saveOptions);
```

### انظر أيضًا

* class [PageSettings](../)
* namespace [Aspose.Tasks.Visualization](../../pagesettings/)
* assembly [Aspose.Tasks](../../../)


