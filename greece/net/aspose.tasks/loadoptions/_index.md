---
title: "Κλάση LoadOptions"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κλάση Aspose.Tasks.LoadOptions. Επιτρέπει τον καθορισμό πρόσθετων παραμέτρων φόρτωσης κατά τη φόρτωση ενός έργου από αρχείο ή ροή."
type: docs
weight: 990
url: /el/net/aspose.tasks/loadoptions/
---
## LoadOptions class

Επιτρέπει τον καθορισμό πρόσθετων παραμέτρων φόρτωσης κατά τη φόρτωση ενός project από αρχείο ή ροή.

```csharp
public class LoadOptions
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [LoadOptions](loadoptions/)() | Αρχικοποιεί μια νέα παρουσία της κλάσης `LoadOptions`. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [CancellationToken](../../aspose.tasks/loadoptions/cancellationtoken/) { get; set; } | Λαμβάνει ή ορίζει ένα διακριτικό που μπορεί να χρησιμοποιηθεί για την ακύρωση μιας λειτουργίας φόρτωσης έργου. |
| [Encoding](../../aspose.tasks/loadoptions/encoding/) { get; set; } | Λαμβάνει ή ορίζει την κωδικοποίηση που χρησιμοποιείται για την ανάγνωση ενός έργου από μορφές HTML, MPX, XER και Primavera XML. Η προεπιλεγμένη κωδικοποίηση είναι UTF8. |
| [ErrorHandler](../../aspose.tasks/loadoptions/errorhandler/) { get; set; } | Λαμβάνει ή ορίζει μια μέθοδο κλήσης για τη διαχείριση σφαλμάτων ανάλυσης XML. |
| [Password](../../aspose.tasks/loadoptions/password/) { get; set; } | Λαμβάνει ή ορίζει έναν κωδικό προστασίας. |
| [PrimaveraReadOptions](../../aspose.tasks/loadoptions/primaverareadoptions/) { get; set; } | Λαμβάνει ή ορίζει μια συγκεκριμένη παρουσία της κλάσης [`PrimaveraReadOptions`](../primaverareadoptions/) που μπορεί να χρησιμοποιηθεί για την προσαρμογή της συμπεριφοράς φόρτωσης μορφών Primavera (Primavera P6 XER ή Primavera P6 Xml). |
| [ProjectLoadingCallback](../../aspose.tasks/loadoptions/projectloadingcallback/) { get; set; } | Λαμβάνει ή ορίζει την κλήση που θα εκτελεστεί κατά τη διάρκεια λειτουργιών φόρτωσης έργου. Υποστηρίζεται επί του παρόντος για μορφές MPP και XER. |

## Παραδείγματα

Δείχνει πώς να φορτώσετε το έργο με προστασία κωδικού χρησιμοποιώντας την παρουσία &lt;see cref=\"Aspose.Tasks.LoadOptions\"/&gt;.

```csharp
using (var stream = new FileStream(DataDir + "PasswordProtectedProject.mpp", FileMode.Open))
{
    var options = new LoadOptions
    {
        Password = "password"
    };
    var project = new Project(stream, options);
    Console.WriteLine(project.Get(Prj.Name));
}
```

### Δείτε επίσης

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


