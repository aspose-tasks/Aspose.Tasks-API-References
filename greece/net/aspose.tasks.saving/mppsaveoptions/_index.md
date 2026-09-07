---
title: "Κλάση MPPSaveOptions"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κλάση Aspose.Tasks.Saving.MPPSaveOptions. Επιτρέπει τον καθορισμό πρόσθετων επιλογών κατά την αποθήκευση των δεδομένων του έργου σε MPP"
type: docs
weight: 2050
url: /el/net/aspose.tasks.saving/mppsaveoptions/
---
## MPPSaveOptions class

Επιτρέπει τον καθορισμό πρόσθετων επιλογών κατά την αποθήκευση των δεδομένων του έργου σε MPP.

```csharp
public class MPPSaveOptions : SimpleSaveOptions
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [MPPSaveOptions](mppsaveoptions/)() | Αρχικοποιεί μια νέα παρουσία της κλάσης `MPPSaveOptions`. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [ClearVba](../../aspose.tasks.saving/mppsaveoptions/clearvba/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν θα αφαιρεθούν τα υπάρχοντα δεδομένα μακροεντολών VBA κατά την αποθήκευση ενός έργου σε μορφή MPP. |
| [ProtectionPassword](../../aspose.tasks.saving/mppsaveoptions/protectionpassword/) { get; set; } | Λαμβάνει ή ορίζει έναν κωδικό πρόσβασης που χρησιμοποιείται για την προστασία του τελικού αρχείου MPP. Προς το παρόν υποστηρίζεται για τα φορμά MS Project 2010 και νεότερα. Μια τιμή null υποδεικνύει ότι το αρχείο έργου δεν είναι προστατευμένο. |
| [RemoveInvalidAssignments](../../aspose.tasks.saving/mppsaveoptions/removeinvalidassignments/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν θα αφαιρεθούν οι μη έγκυρες εκχωρήσεις πόρων κατά την αποθήκευση σε MPP. Το MS Project δημιουργεί μια κενή εκχώρηση πόρου για κάθε εργασία. Ορίστε αυτή τη σημαία σε true για να τις αφαιρέσετε κατά την αποθήκευση. |
| [SaveFormat](../../aspose.tasks.saving/simplesaveoptions/saveformat/) { get; } | Λαμβάνει ή ορίζει τη μορφή στην οποία θα αποθηκευτεί το έγγραφο εάν χρησιμοποιηθεί αυτό το αντικείμενο επιλογών αποθήκευσης. |
| [TasksComparer](../../aspose.tasks.saving/simplesaveoptions/taskscomparer/) { get; set; } | Λαμβάνει ή ορίζει τον συγκριτή για την ταξινόμηση των εργασιών στο γράφημα Gantt και στο γράφημα Φύλλου Εργασιών. |
| [TasksFilter](../../aspose.tasks.saving/simplesaveoptions/tasksfilter/) { get; set; } | Λαμβάνει ή ορίζει τη συνθήκη που χρησιμοποιείται για το φιλτράρισμα των εργασιών που αποδίδονται στα γραφήματα Gantt, Φύλλο Εργασιών και Χρήση Εργασιών. |
| [WriteFilters](../../aspose.tasks.saving/mppsaveoptions/writefilters/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν θα γραφτούν τα δεδομένα φίλτρων κατά την αποθήκευση ενός έργου σε μορφή MPP. Τα δεδομένα φίλτρων περιλαμβάνουν τις συλλογές Project.TaskFilters και Project.ResourceFilters. |
| [WriteGroups](../../aspose.tasks.saving/mppsaveoptions/writegroups/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν θα γραφτούν τα δεδομένα ομάδων κατά την αποθήκευση ενός έργου σε μορφή MPP. Τα δεδομένα ομάδων περιλαμβάνουν τις συλλογές Project.TaskGroups και Project.ResourceGroups. |
| [WriteVba](../../aspose.tasks.saving/mppsaveoptions/writevba/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν θα ενημερωθούν τα υπάρχοντα δεδομένα μακροεντολών VBA στο αρχείο MPP. Προς το παρόν υποστηρίζεται η εγγραφή του VbaModule.SourceCode. |
| [WriteViewData](../../aspose.tasks.saving/mppsaveoptions/writeviewdata/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν θα γραφτούν τα δεδομένα προβολής κατά την αποθήκευση ενός έργου σε μορφή MPP. Τα δεδομένα προβολής περιλαμβάνουν τις συλλογές Project.Views, Filters και Tables. |

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

* class [SimpleSaveOptions](../simplesaveoptions/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


