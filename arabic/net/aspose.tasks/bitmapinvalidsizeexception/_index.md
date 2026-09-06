---
title: "فئة BitmapInvalidSizeException"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "فئة Aspose.Tasks.BitmapInvalidSizeException. تمثل الاستثناء الذي يحدث عندما لا توجد ذاكرة كافية لإنشاء نسخة bitmap."
type: docs
weight: 140
url: /ar/net/aspose.tasks/bitmapinvalidsizeexception/
---
## BitmapInvalidSizeException class

يمثل استثناء يحدث عندما لا توجد ذاكرة كافية لإنشاء نسخة من bitmap.

```csharp
public class BitmapInvalidSizeException : Exception
```

## الأمثلة

يظهر كيفية حفظ المشروع كصورة والتقاط استثناء الحجم غير الصالح.

```csharp
try
{
    var project = new Project(DataDir + "Blank2010.mpp");

    GanttChartView view = (GanttChartView) project.Views.ToList()[0];
    var options = new ImageSaveOptions(SaveFileFormat.Png)
    {
        Timescale = Timescale.DefinedInView
    };

    view.MiddleTimescaleTier.Unit = TimescaleUnit.Minutes;
    view.MiddleTimescaleTier.Count = 1;

    project.Save(OutDir + "SaveToStreamAndCatchException_out.mpp", options);
}
catch (BitmapInvalidSizeException ex)
{
    Console.WriteLine(ex.Message);
}
```

### انظر أيضًا

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


