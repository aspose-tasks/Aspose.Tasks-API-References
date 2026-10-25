---
title: "SaveOptions.RollUpGanttBars"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية SaveOptions. تحصل أو تعين قيمة تشير إلى ما إذا كان يجب تمييز المهام الفرعية على شريط المهمة الملخصة. بالنسبة للمهام الفرعية، حقل Rollup يشير إلى ما إذا كانت معلومات أشرطة Gantt للمهام الفرعية ستُدمج في شريط المهمة الملخصة. بالنسبة للمهام الملخصة، حقل Rollup يشير إلى ما إذا كان شريط المهمة الملخصة يعرض أشرطة مدمجة. يجب أن يكون حقل Rollup للمهام الملخصة مضبوطًا على نعم لأي مهام فرعية لتُدمج فيها"
type: docs
weight: 160
url: /ar/net/aspose.tasks.saving/saveoptions/rollupganttbars/
---
## SaveOptions.RollUpGanttBars property

يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب وضع علامة على المهام الفرعية في شريط مهمة الملخص. بالنسبة للمهام الفرعية، يشير حقل Rollup إلى ما إذا كانت معلومات أشرطة جانت للمهام الفرعية ستُدمج في شريط مهمة الملخص. بالنسبة لمهام الملخص، يشير حقل Rollup إلى ما إذا كان شريط مهمة الملخص يعرض أشرطة مدمجة. يجب أن يكون حقل Rollup لمهام الملخص مضبوطًا على Yes لتتمكن أي مهام فرعية من الدمج معها.

```csharp
public bool RollUpGanttBars { get; set; }
```

## ملاحظات

يُطبق فقط عندما يتم تصوير عرض مخطط Gantt.

## الأمثلة

يظهر كيفية تعيين قيمة تشير إلى أن المهام الفرعية على شريط مهمة الملخص يجب تجميعها.

```csharp
var project = new Project(DataDir + "Project2.mpp");

project.DisplayOptions.ShowProjectSummaryTask = true;
project.Set(Prj.ShowProjectSummaryTask, true);

var options = new PdfSaveOptions
{
    PresentationFormat = PresentationFormat.GanttChart,
    FitContent = true,
    RollUpGanttBars = true,

    // أو
    // options.RollUpGanttBars = false;
    // DrawNonWorkingTime = true,
    PageSize = PageSize.A3
};

project.Save(OutDir + "RenderGanttChartWithBarsRolledUp_out.pdf", options);
```

### انظر أيضًا

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


