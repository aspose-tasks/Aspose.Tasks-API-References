---
title: "Κλάση PrimaveraSaveOptions"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.Saving.PrimaveraSaveOptions class. Επιτρέπει τον καθορισμό πρόσθετων επιλογών κατά την αποθήκευση του έργου σε μορφή Primavera XER"
type: docs
weight: 2150
url: /el/net/aspose.tasks.saving/primaverasaveoptions/
---
## PrimaveraSaveOptions class

Επιτρέπει τον καθορισμό πρόσθετων επιλογών κατά την αποθήκευση του έργου σε μορφή Primavera XER.

```csharp
public class PrimaveraSaveOptions : SimpleSaveOptions
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [PrimaveraSaveOptions](primaverasaveoptions/)() | Αρχικοποιεί μια νέα παρουσία της κλάσης `PrimaveraSaveOptions`. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [ActivityIdIncrement](../../aspose.tasks.saving/primaverasaveoptions/activityidincrement/) { get; set; } | Λαμβάνει ή ορίζει την αύξηση που χρησιμοποιείται στην επανααρίθμηση των αναγνωριστικών δραστηριότητας. |
| [ActivityIdPrefix](../../aspose.tasks.saving/primaverasaveoptions/activityidprefix/) { get; set; } | Λαμβάνει ή ορίζει το πρόθεμα που χρησιμοποιείται στην επανααρίθμηση των αναγνωριστικών δραστηριότητας. |
| [ActivityIdSuffix](../../aspose.tasks.saving/primaverasaveoptions/activityidsuffix/) { get; set; } | Λαμβάνει ή ορίζει το επίθημα που χρησιμοποιείται στην επανααρίθμηση των αναγνωριστικών δραστηριότητας. |
| [RenumberActivityIds](../../aspose.tasks.saving/primaverasaveoptions/renumberactivityids/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν χρειάζεται η επανααρίθμηση των αναγνωριστικών δραστηριότητας. |
| [SaveFormat](../../aspose.tasks.saving/simplesaveoptions/saveformat/) { get; } | Λαμβάνει ή ορίζει τη μορφή στην οποία θα αποθηκευτεί το έγγραφο εάν χρησιμοποιηθεί αυτό το αντικείμενο επιλογών αποθήκευσης. |
| [SkipSummaryAssignments](../../aspose.tasks.saving/primaverasaveoptions/skipsummaryassignments/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει αν οι εκχωρήσεις πόρων σε συνοπτικές εργασίες πρέπει να παραλειφθούν κατά την εξαγωγή. |
| [TasksComparer](../../aspose.tasks.saving/simplesaveoptions/taskscomparer/) { get; set; } | Λαμβάνει ή ορίζει τον συγκριτή για την ταξινόμηση των εργασιών στο γράφημα Gantt και στο γράφημα Φύλλου Εργασιών. |
| [TasksFilter](../../aspose.tasks.saving/simplesaveoptions/tasksfilter/) { get; set; } | Λαμβάνει ή ορίζει τη συνθήκη που χρησιμοποιείται για το φιλτράρισμα των εργασιών που αποδίδονται στα γραφήματα Gantt, Φύλλο Εργασιών και Χρήση Εργασιών. |

## Παραδείγματα

Δείχνει πώς να εργαστείτε με &lt;see cref="Aspose.Tasks.Saving.PrimaveraSaveOptions" /&gt;.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// Δημιουργήστε επιλογές αποθήκευσης Primavera και ρυθμίστε τις
var options = new PrimaveraSaveOptions
                  {
                      // ορίστε πρόθεμα και επίθημα μιας δραστηριότητας
                      ActivityIdPrefix = "TEST",
                      ActivityIdSuffix = 10000,

                      // ελέγξτε την επανααρίθμηση των δραστηριοτήτων
                      ActivityIdIncrement = 5,
                      RenumberActivityIds = true
                  };

project.Save(OutDir + "WorkWithPrimaveraSaveOptions_out.xer", options);
```

### Δείτε επίσης

* class [SimpleSaveOptions](../simplesaveoptions/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


