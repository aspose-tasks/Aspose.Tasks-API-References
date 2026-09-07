---
title: "Κλάση ApsLayoutBuilderOutOfMemoryException"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κλάση Aspose.Tasks.ApsLayoutBuilderOutOfMemoryException. Αντιπροσωπεύει την εξαίρεση που συμβαίνει όταν δεν υπάρχει αρκετή μνήμη για να συνεχιστεί η δημιουργία διάταξης εικόνας"
type: docs
weight: 20
url: /el/net/aspose.tasks/apslayoutbuilderoutofmemoryexception/
---
## ApsLayoutBuilderOutOfMemoryException class

Αντιπροσωπεύει εξαίρεση που συμβαίνει όταν δεν υπάρχει αρκετή μνήμη για να συνεχιστεί η δημιουργία διάταξης εικόνας.

```csharp
public class ApsLayoutBuilderOutOfMemoryException : Exception
```

## Παραδείγματα

Δείχνει πώς να αποθηκεύσετε το έργο ως εικόνα και να πιάσετε εξαιρέσεις.

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

### Δείτε επίσης

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


