---
title: "MPPSaveOptions.RemoveInvalidAssignments"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα MPPSaveOptions. Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν θα αφαιρεθούν μη έγκυρες εκχωρήσεις πόρων κατά την αποθήκευση σε MPP. Το MS Project δημιουργεί μια κενή εκχώρηση πόρου για κάθε εργασία. Ορίστε αυτή τη σημαία σε true για να τις αφαιρέσετε κατά την αποθήκευση."
type: docs
weight: 40
url: /el/net/aspose.tasks.saving/mppsaveoptions/removeinvalidassignments/
---
## MPPSaveOptions.RemoveInvalidAssignments property

Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν θα αφαιρεθούν οι μη έγκυρες εκχωρήσεις πόρων κατά την αποθήκευση σε MPP. Το MS Project δημιουργεί μια κενή εκχώρηση πόρου για κάθε εργασία. Ορίστε αυτή τη σημαία σε true για να τις αφαιρέσετε κατά την αποθήκευση.

```csharp
public bool RemoveInvalidAssignments { get; set; }
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


