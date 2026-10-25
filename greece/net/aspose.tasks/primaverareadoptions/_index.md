---
title: "Κλάση PrimaveraReadOptions"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κλάση Aspose.Tasks.PrimaveraReadOptions. Επιτρέπει τον καθορισμό πρόσθετων επιλογών κατά την ανάγνωση αρχείων Primavera Xml ή Primavera Xer."
type: docs
weight: 1370
url: /el/net/aspose.tasks/primaverareadoptions/
---
## PrimaveraReadOptions class

Επιτρέπει τον καθορισμό πρόσθετων επιλογών κατά την ανάγνωση αρχείων Primavera Xml ή Primavera Xer.

```csharp
public class PrimaveraReadOptions
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [PrimaveraReadOptions](primaverareadoptions/)() | Αρχικοποιεί μια νέα παρουσία της κλάσης `PrimaveraReadOptions`. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [PreserveUids](../../aspose.tasks/primaverareadoptions/preserveuids/) { get; set; } | Λαμβάνει ή ορίζει μια σημαία που καθορίζει εάν τα αρχικά μοναδικά αναγνωριστικά των οντοτήτων πρέπει να διατηρηθούν. |
| [ProjectUid](../../aspose.tasks/primaverareadoptions/projectuid/) { get; set; } | Λαμβάνει ή ορίζει το UID ενός έργου για ανάγνωση από αρχείο που περιέχει πολλαπλά έργα. |
| [ReadBaselineProjects](../../aspose.tasks/primaverareadoptions/readbaselineprojects/) { get; set; } | Λαμβάνει ή ορίζει μια σημαία που καθορίζει εάν τα βασικά (baseline) έργα πρέπει να φορτωθούν. Η προεπιλεγμένη τιμή είναι true. |
| [UndefinedConstraintHandlingBehavior](../../aspose.tasks/primaverareadoptions/undefinedconstrainthandlingbehavior/) { get; set; } | Καθορίζει τη συμπεριφορά που χρησιμοποιείται για την επεξεργασία εργασιών με ακαθόριστους περιορισμούς που διαβάζονται από μορφή XER. |

## Παραδείγματα

Δείχνει πώς να διαβάσετε ένα έργο από αρχείο Primavera XML ή Primavera XER που περιέχει πολλαπλά έργα.

```csharp
var options = new PrimaveraReadOptions();
options.ProjectUid = 3881;

// Επιστρέφει έργο με ειδικό UID
var project = new Project(DataDir + "PrimaveraProject.xml", options);
Console.WriteLine(project.Get(Prj.Name));
```

### Δείτε επίσης

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


