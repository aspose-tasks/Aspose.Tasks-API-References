---
title: "SimpleSaveOptions.TasksFilter"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα SimpleSaveOptions. Λαμβάνει ή ορίζει τη συνθήκη που χρησιμοποιείται για το φιλτράρισμα των εργασιών που εμφανίζονται στο φύλλο Gantt Task Sheet και στα διαγράμματα χρήσης εργασιών"
type: docs
weight: 30
url: /el/net/aspose.tasks.saving/simplesaveoptions/tasksfilter/
---
## SimpleSaveOptions.TasksFilter property

Λαμβάνει ή ορίζει τη συνθήκη που χρησιμοποιείται για το φιλτράρισμα των εργασιών που αποδίδονται στα γραφήματα Gantt, Φύλλο Εργασιών και Χρήση Εργασιών.

```csharp
public ICondition<Task> TasksFilter { get; set; }
```

## Παρατηρήσεις

Εάν η τιμή δεν καθοριστεί, χρησιμοποιείται το προεπιλεγμένο φίλτρο που αφαιρεί τις μη ορατές εργασίες — δηλαδή τις υποεργασίες των συμπτυγμένων εργασιών.

## Παραδείγματα

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

* interface [ICondition&lt;T&gt;](../../../aspose.tasks.util/icondition-1/)
* class [Task](../../../aspose.tasks/task/)
* class [SimpleSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../simplesaveoptions/)
* assembly [Aspose.Tasks](../../../)


