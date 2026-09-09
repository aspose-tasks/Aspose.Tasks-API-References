---
title: "Sınıf BitmapInvalidSizeException"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.BitmapInvalidSizeException sınıfı. Yeterli bellek olmadığında bir bitmap örneği oluşturulurken oluşan istisnayı temsil eder."
type: docs
weight: 140
url: /tr/net/aspose.tasks/bitmapinvalidsizeexception/
---
## BitmapInvalidSizeException class

Bitmap örneği oluşturmak için yeterli bellek olmadığında oluşan istisnayı temsil eder.

```csharp
public class BitmapInvalidSizeException : Exception
```

## Örnekler

Projeyi bir görüntü olarak kaydetme ve geçersiz boyut istisnasını yakalama yöntemini gösterir.

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

### Ayrıca Bakınız

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


