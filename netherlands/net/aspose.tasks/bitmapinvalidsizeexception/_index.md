---
title: "Class BitmapInvalidSizeException"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.BitmapInvalidSizeException class. Vertegenwoordigt een uitzondering die optreedt wanneer er niet genoeg geheugen is om een bitmap‑instantie te maken"
type: docs
weight: 140
url: /nl/net/aspose.tasks/bitmapinvalidsizeexception/
---
## BitmapInvalidSizeException class

Stelt een uitzondering voor die optreedt wanneer er niet genoeg geheugen is om een bitmap‑instantie te maken.

```csharp
public class BitmapInvalidSizeException : Exception
```

## Voorbeelden

Toont hoe je een project opslaat als een afbeelding en een ongeldige grootte‑uitzondering afhandelt.

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

### Zie ook

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


