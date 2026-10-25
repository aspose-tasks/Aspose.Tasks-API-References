---
title: "Clase BitmapInvalidSizeException"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.BitmapInvalidSizeException. Representa la excepción que ocurre cuando no hay suficiente memoria para crear una instancia de bitmap"
type: docs
weight: 140
url: /es/net/aspose.tasks/bitmapinvalidsizeexception/
---
## BitmapInvalidSizeException class

Representa la excepción que ocurre cuando no hay suficiente memoria para crear una instancia de mapa de bits.

```csharp
public class BitmapInvalidSizeException : Exception
```

## Ejemplos

Muestra cómo guardar el proyecto como una imagen y capturar la excepción de tamaño inválido.

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

### Ver también

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


