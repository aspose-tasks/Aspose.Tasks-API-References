---
title: "Класс BitmapInvalidSizeException"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.BitmapInvalidSizeException. Представляет исключение, которое возникает, когда недостаточно памяти для создания экземпляра bitmap."
type: docs
weight: 140
url: /ru/net/aspose.tasks/bitmapinvalidsizeexception/
---
## BitmapInvalidSizeException class

Представляет исключение, которое происходит, когда недостаточно памяти для создания экземпляра bitmap.

```csharp
public class BitmapInvalidSizeException : Exception
```

## Примеры

Показывает, как сохранить проект как изображение и обработать исключение неверного размера.

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

### См. также

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


