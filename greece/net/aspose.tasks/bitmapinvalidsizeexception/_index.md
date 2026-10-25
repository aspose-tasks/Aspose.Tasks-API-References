---
title: "Κλάση BitmapInvalidSizeException"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κλάση Aspose.Tasks.BitmapInvalidSizeException. Αντιπροσωπεύει την εξαίρεση που εμφανίζεται όταν δεν υπάρχει αρκετή μνήμη για τη δημιουργία ενός αντικειμένου bitmap"
type: docs
weight: 140
url: /el/net/aspose.tasks/bitmapinvalidsizeexception/
---
## BitmapInvalidSizeException class

Αντιπροσωπεύει την εξαίρεση που εμφανίζεται όταν δεν υπάρχει αρκετή μνήμη για τη δημιουργία μιας εμφάνισης bitmap.

```csharp
public class BitmapInvalidSizeException : Exception
```

## Παραδείγματα

Δείχνει πώς να αποθηκεύσετε το έργο ως εικόνα και να πιάσετε την εξαίρεση μη έγκυρου μεγέθους.

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

### Δείτε επίσης

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


