---
title: "Classe ApsLayoutBuilderOutOfMemoryException"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.ApsLayoutBuilderOutOfMemoryException. Rappresenta un'eccezione che si verifica quando non c'è abbastanza memoria per continuare la costruzione del layout dell'immagine"
type: docs
weight: 20
url: /it/net/aspose.tasks/apslayoutbuilderoutofmemoryexception/
---
## ApsLayoutBuilderOutOfMemoryException class

Rappresenta l'eccezione che si verifica quando non c'è abbastanza memoria per continuare la costruzione del layout dell'immagine.

```csharp
public class ApsLayoutBuilderOutOfMemoryException : Exception
```

## Esempi

Mostra come salvare il progetto come immagine e gestire le eccezioni.

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

### Vedi anche

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


