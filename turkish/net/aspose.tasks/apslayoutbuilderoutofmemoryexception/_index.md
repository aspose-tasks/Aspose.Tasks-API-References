---
title: "Sınıf ApsLayoutBuilderOutOfMemoryException"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.ApsLayoutBuilderOutOfMemoryException sınıfı. Görüntü yerleşimi oluşturulmasına devam etmek için yeterli bellek olmadığında oluşan bir istisnayı temsil eder"
type: docs
weight: 20
url: /tr/net/aspose.tasks/apslayoutbuilderoutofmemoryexception/
---
## ApsLayoutBuilderOutOfMemoryException class

Görüntü düzeni oluşturulmasına devam etmek için yeterli bellek olmadığında oluşan istisnayı temsil eder.

```csharp
public class ApsLayoutBuilderOutOfMemoryException : Exception
```

## Örnekler

Projenin bir görüntü olarak nasıl kaydedileceğini ve istisnaların nasıl yakalanacağını gösterir.

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

### Ayrıca Bakınız

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


