---
title: "PageSettings.AdjustToPercentOfNormalSize"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية PageSettings. تحصل أو تضبط قيمة تشير إلى ما إذا كان يجب ضبط الطباعة إلى النسبة المئوية المحددة PercentOfNormalSize من الحجم الطبيعي"
type: docs
weight: 20
url: /ar/net/aspose.tasks.visualization/pagesettings/adjusttopercentofnormalsize/
---
## PageSettings.AdjustToPercentOfNormalSize property

تحصل أو تضبط قيمة تشير إلى ما إذا كان يجب ضبط الطباعة إلى النسبة المئوية المحددة ([`PercentOfNormalSize`](../percentofnormalsize/)) من الحجم الطبيعي.

```csharp
public bool AdjustToPercentOfNormalSize { get; set; }
```

## ملاحظات

ليس فعالًا عندما يتم عرض المشروع بتنسيق HTML.

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


