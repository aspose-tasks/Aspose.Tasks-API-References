---
title: "Klasse ApsLayoutBuilderOutOfMemoryException"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.ApsLayoutBuilderOutOfMemoryException klasse. Vertegenwoordigt een uitzondering die optreedt wanneer er niet genoeg geheugen is om het bouwen van een afbeeldingslay-out voort te zetten"
type: docs
weight: 20
url: /nl/net/aspose.tasks/apslayoutbuilderoutofmemoryexception/
---
## ApsLayoutBuilderOutOfMemoryException class

Stelt een uitzondering voor die optreedt wanneer er niet genoeg geheugen is om het bouwen van een afbeeldingslay-out voort te zetten.

```csharp
public class ApsLayoutBuilderOutOfMemoryException : Exception
```

## Voorbeelden

Toont hoe een project als afbeelding op te slaan en uitzonderingen af te handelen.

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

### Zie ook

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


