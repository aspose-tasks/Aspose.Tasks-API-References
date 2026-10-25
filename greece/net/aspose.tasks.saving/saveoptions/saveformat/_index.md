---
title: "SaveFormat"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Λαμβάνει ή ορίζει τη μορφή στην οποία θα αποθηκευτεί το έγγραφο εάν χρησιμοποιηθεί αυτό το αντικείμενο επιλογών αποθήκευσης."
type: docs
weight: 160
url: /el/net/aspose.tasks.saving/saveoptions/saveformat/
---
## SaveOptions.SaveFormat property

Λαμβάνει ή ορίζει τη μορφή στην οποία θα αποθηκευτεί το έγγραφο εάν χρησιμοποιηθεί αυτό το αντικείμενο επιλογών αποθήκευσης.

```csharp
public SaveFileFormat SaveFormat { get; }
```

### Παραδείγματα

Δείχνει πώς να χρησιμοποιήσετε προσαρμοσμένο φίλτρο εργασιών κατά την αποθήκευση του αρχείου MS Project.

```csharp
public void WorkWithTasksFilter()
{
    var project = new Project(DataDir + "CreateProject2.mpp");

    var options = new PdfSaveOptions
    {
        PresentationFormat = PresentationFormat.GanttChart,
        PageSize = PageSize.A3,
        StartDate = new DateTime(2010, 7, 1),
        EndDate = new DateTime(2010, 9, 1),

        // ορίστε ένα φίλτρο εργασίας για να παραλείψετε την εργασία 'Task5' και 'Task3'
        TasksFilter = new CustomTasksFilter()
    };

    // ας ελέγξουμε τη μορφή αποθήκευσης
    Console.WriteLine("The save format: " + options.SaveFormat);

    // ...

    // αποθηκεύστε το έργο ως εικόνα
    project.Save(OutDir + "WorkWithTasksFilter_out.png", options);
}

/// <summary>
/// Παράδειγμα προσαρμοσμένου φίλτρου εργασιών που μπορεί να χρησιμοποιηθεί κατά την αποθήκευση του αρχείου MS Project (για παράδειγμα) σε μορφή PDF.
/// </summary>
/// <inheritdoc />
private class CustomTasksFilter : ICondition<Task>
{
    public bool Check(Task el)
    {
        return el.Get(Tsk.Name) != "Task5" && el.Get(Tsk.Name) != "Task3";
    }
}
```

### Δείτε επίσης

* enum [SaveFileFormat](../../savefileformat)
* class [SaveOptions](../../saveoptions)
* namespace [Aspose.Tasks.Saving](../../saveoptions)
* assembly [Aspose.Tasks](../../../)

<!-- ΜΗ ΕΠΕΞΕΡΓΑΣΙΑ: δημιουργήθηκε από xmldocmd για Aspose.Tasks.dll -->
