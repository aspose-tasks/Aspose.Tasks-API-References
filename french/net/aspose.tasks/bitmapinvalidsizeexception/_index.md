---
title: "Class BitmapInvalidSizeException"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.BitmapInvalidSizeException. Représente l'exception qui se produit lorsqu'il n'y a pas suffisamment de mémoire pour créer une instance de bitmap."
type: docs
weight: 140
url: /fr/net/aspose.tasks/bitmapinvalidsizeexception/
---
## BitmapInvalidSizeException class

Représente l'exception qui se produit lorsqu'il n'y a pas suffisamment de mémoire pour créer une instance bitmap.

```csharp
public class BitmapInvalidSizeException : Exception
```

## Exemples

Montre comment enregistrer le projet en tant qu'image et intercepter l'exception de taille invalide.

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

### Voir aussi

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


