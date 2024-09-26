---
title: Class BitmapInvalidSizeException
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.BitmapInvalidSizeException class. Represents exception which occurs when there is not enough memory to create a bitmap instance
type: docs
weight: 140
url: /net/aspose.tasks/bitmapinvalidsizeexception/
---
## BitmapInvalidSizeException class

Represents exception which occurs when there is not enough memory to create a bitmap instance.

```csharp
public class BitmapInvalidSizeException : Exception
```

## Examples

Shows how to save project as an image and catch invalid size exception.

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

### See Also

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


