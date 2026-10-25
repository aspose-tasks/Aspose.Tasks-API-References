---
title: "Κλάση ProjectFileInfo"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κλάση Aspose.Tasks.ProjectFileInfo. Η παρουσία της κλάσης περιέχει πληροφορίες σχετικά με τη μορφή του αρχείου έργου και την έκδοση του Microsoft Project όπου δημιουργήθηκε το αρχείο."
type: docs
weight: 1460
url: /el/net/aspose.tasks/projectfileinfo/
---
## ProjectFileInfo class

Η παρουσία της κλάσης περιέχει πληροφορίες σχετικά με τη μορφή αρχείου έργου και την έκδοση του Microsoft Project όπου δημιουργήθηκε το αρχείο.

```csharp
public sealed class ProjectFileInfo : IEquatable<ProjectFileInfo>
```

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [CanRead](../../aspose.tasks/projectfileinfo/canread/) { get; } | Επιστρέφει μια τιμή που υποδεικνύει εάν το Aspose.Tasks μπορεί να επεξεργαστεί το αρχείο έργου. |
| [IsPasswordProtected](../../aspose.tasks/projectfileinfo/ispasswordprotected/) { get; } | Επιστρέφει μια τιμή που υποδεικνύει εάν ένα έργο είναι προστατευμένο με κωδικό. |
| [ProjectApplicationInfo](../../aspose.tasks/projectfileinfo/projectapplicationinfo/) { get; } | Επιστρέφει πληροφορίες εφαρμογής του αρχείου έργου. |
| [ProjectFileFormat](../../aspose.tasks/projectfileinfo/projectfileformat/) { get; } | Επιστρέφει τη μορφή του αρχείου έργου. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| override [Equals](../../aspose.tasks/projectfileinfo/equals/#equals_1)(object) | Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι ίση με ένα καθορισμένο αντικείμενο. |
| [Equals](../../aspose.tasks/projectfileinfo/equals/#equals)(ProjectFileInfo) | Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι ίση με ένα καθορισμένο αντικείμενο. |
| override [GetHashCode](../../aspose.tasks/projectfileinfo/gethashcode/)() | Επιστρέφει μια τιμή κώδικα κατακερματισμού για την παρουσία της κλάσης `ProjectFileInfo`. |

## Παρατηρήσεις

Χρησιμοποιήστε την ιδιότητα CanRead για να ορίσετε ότι η βιβλιοθήκη μπορεί να επεξεργαστεί το αρχείο έργου.

## Παραδείγματα

Δείχνει πώς να διαβάσετε τις πληροφορίες του αρχείου έργου.

```csharp
var info = Project.GetProjectFileInfo(DataDir + "Project.xml");
Console.WriteLine("CanRead: " + info.CanRead);
Console.WriteLine("ProjectApplicationInfo: " + info.ProjectApplicationInfo);
Console.WriteLine("ProjectFileFormat: " + info.ProjectFileFormat);
```

### Δείτε επίσης

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


