---
title: "Класс ApsLayoutBuilderOutOfMemoryException"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.ApsLayoutBuilderOutOfMemoryException. Представляет исключение, которое возникает, когда недостаточно памяти для продолжения построения макета изображения"
type: docs
weight: 20
url: /ru/net/aspose.tasks/apslayoutbuilderoutofmemoryexception/
---
## ApsLayoutBuilderOutOfMemoryException class

Представляет исключение, которое возникает, когда недостаточно памяти для продолжения построения компоновки изображения.

```csharp
public class ApsLayoutBuilderOutOfMemoryException : Exception
```

## Примеры

Показывает, как сохранить проект как изображение и обработать исключения.

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

### См. также

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


