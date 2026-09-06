---
title: "الفئة ApsLayoutBuilderOutOfMemoryException"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.ApsLayoutBuilderOutOfMemoryException. تمثل استثناء يحدث عندما لا توجد ذاكرة كافية لمتابعة بناء تخطيط الصورة"
type: docs
weight: 20
url: /ar/net/aspose.tasks/apslayoutbuilderoutofmemoryexception/
---
## ApsLayoutBuilderOutOfMemoryException class

يمثل الاستثناء الذي يحدث عندما لا توجد ذاكرة كافية لمتابعة بناء تخطيط الصورة.

```csharp
public class ApsLayoutBuilderOutOfMemoryException : Exception
```

## الأمثلة

يظهر كيفية حفظ المشروع كصورة والتقاط الاستثناءات.

```csharp
try
{
    var project = new Project(DataDir + "Blank2010.mpp");

    var ganttChart = (GanttChartView)project.Views.ToList()[0];

    ganttChart.MiddleTimescaleTier.Unit = TimescaleUnit.Hours;
    ganttChart.BottomTimescaleTier.Unit = TimescaleUnit.Minutes;
    ganttChart.BottomTimescaleTier.Count = 1;

    var options = new ImageSaveOptions(SaveFileFormat.Png);
    options.Timescale = Timescale.DefinedInView;

    project.Save(OutDir + "SaveToStreamWithOptionsAndCatchException_out.mpp", options);
}
catch (ApsLayoutBuilderOutOfMemoryException ex)
{
    Console.WriteLine(ex.Message);
}
catch (BitmapInvalidSizeException ex)
{
    Console.WriteLine(ex.Message);
}
```

### انظر أيضًا

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


