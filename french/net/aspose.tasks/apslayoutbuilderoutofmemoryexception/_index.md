---
title: "Classe ApsLayoutBuilderOutOfMemoryException"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.ApsLayoutBuilderOutOfMemoryException. Représente l'exception qui se produit lorsqu'il n'y a pas assez de mémoire pour poursuivre la construction d'une mise en page d'image"
type: docs
weight: 20
url: /fr/net/aspose.tasks/apslayoutbuilderoutofmemoryexception/
---
## ApsLayoutBuilderOutOfMemoryException class

Représente une exception qui se produit lorsqu'il n'y a pas suffisamment de mémoire pour poursuivre la construction de la mise en page d'image.

```csharp
public class ApsLayoutBuilderOutOfMemoryException : Exception
```

## Exemples

Montre comment enregistrer le projet en tant qu'image et intercepter les exceptions.

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

### Voir aussi

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


