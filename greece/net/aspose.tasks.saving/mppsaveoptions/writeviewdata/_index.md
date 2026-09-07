---
title: "MPPSaveOptions.WriteViewData"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα MPPSaveOptions. Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν θα γραφτούν τα δεδομένα προβολής κατά την αποθήκευση ενός έργου σε μορφή MPP. Τα δεδομένα προβολής περιλαμβάνουν τις συλλογές Project.Views, Filters και Tables."
type: docs
weight: 80
url: /el/net/aspose.tasks.saving/mppsaveoptions/writeviewdata/
---
## MPPSaveOptions.WriteViewData property

Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν θα γραφτούν τα δεδομένα προβολής κατά την αποθήκευση ενός έργου σε μορφή MPP. Τα δεδομένα προβολής περιλαμβάνουν τις συλλογές Project.Views, Filters και Tables.

```csharp
public bool WriteViewData { get; set; }
```

## Παραδείγματα

Δείχνει πώς να αποθηκεύσετε το έργο σε μια ροή ως αρχείο MPP.

```csharp
using (var stream = new FileStream(OutDir + "EmptyProjectSaveStream_out.xml", FileMode.Create, FileAccess.Write))
{
    var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

    // δημιουργία επιλογών αποθήκευσης
    SimpleSaveOptions options = new MPPSaveOptions
    {
        // ορίζει μια τιμή που υποδεικνύει εάν θα αφαιρεθούν οι μη έγκυρες εκχωρήσεις πόρων κατά την αποθήκευση σε MPP
        RemoveInvalidAssignments = true
    };

    // αποθήκευση MPP με επιλογές
    project.Save(stream, options);
}
```

### Δείτε επίσης

* class [MPPSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../mppsaveoptions/)
* assembly [Aspose.Tasks](../../../)


