---
title: "Classe BitmapInvalidSizeException"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.BitmapInvalidSizeException. Rappresenta l'eccezione che si verifica quando non c'è abbastanza memoria per creare un'istanza bitmap."
type: docs
weight: 140
url: /it/net/aspose.tasks/bitmapinvalidsizeexception/
---
## BitmapInvalidSizeException class

Rappresenta l'eccezione che si verifica quando non c'è abbastanza memoria per creare un'istanza bitmap.

```csharp
public class BitmapInvalidSizeException : Exception
```

## Esempi

Mostra come salvare il progetto come immagine e gestire l'eccezione di dimensione non valida.

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

### Vedi anche

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


