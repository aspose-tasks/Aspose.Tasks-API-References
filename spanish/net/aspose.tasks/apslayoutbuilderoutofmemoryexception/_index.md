---
title: "Clase ApsLayoutBuilderOutOfMemoryException"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.ApsLayoutBuilderOutOfMemoryException. Representa una excepción que ocurre cuando no hay suficiente memoria para continuar la construcción del diseño de la imagen"
type: docs
weight: 20
url: /es/net/aspose.tasks/apslayoutbuilderoutofmemoryexception/
---
## ApsLayoutBuilderOutOfMemoryException class

Representa una excepción que ocurre cuando no hay suficiente memoria para continuar la construcción del diseño de la imagen.

```csharp
public class ApsLayoutBuilderOutOfMemoryException : Exception
```

## Ejemplos

Muestra cómo guardar el proyecto como una imagen y capturar excepciones.

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

### Ver también

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


