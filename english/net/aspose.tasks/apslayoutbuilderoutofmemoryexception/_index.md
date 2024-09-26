---
title: Class ApsLayoutBuilderOutOfMemoryException
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.ApsLayoutBuilderOutOfMemoryException class. Represents exception which occurs when there is not enough memory to continue an image layout building
type: docs
weight: 20
url: /net/aspose.tasks/apslayoutbuilderoutofmemoryexception/
---
## ApsLayoutBuilderOutOfMemoryException class

Represents exception which occurs when there is not enough memory to continue an image layout building.

```csharp
public class ApsLayoutBuilderOutOfMemoryException : Exception
```

## Examples

Shows how to save project as an image and catch exceptions.

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

### See Also

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


