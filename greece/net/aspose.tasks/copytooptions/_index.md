---
title: "Κλάση CopyToOptions"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κλάση Aspose.Tasks.CopyToOptions. Επιτρέπει τον καθορισμό πρόσθετων επιλογών κατά την αντιγραφή δεδομένων έργου"
type: docs
weight: 340
url: /el/net/aspose.tasks/copytooptions/
---
## CopyToOptions class

Επιτρέπει τον καθορισμό πρόσθετων επιλογών κατά την αντιγραφή δεδομένων έργου.

```csharp
public class CopyToOptions
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [CopyToOptions](copytooptions/)() | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης `CopyToOptions`. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [CopyViewData](../../aspose.tasks/copytooptions/copyviewdata/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει αν θα αντιγραφούν τα δεδομένα προβολής κατά την αντιγραφή δεδομένων έργου. Η προεπιλεγμένη τιμή είναι true. |

## Παραδείγματα

Δείχνει πώς να χρησιμοποιήσετε τις επιλογές αντιγραφής έργου.

```csharp
var project = new Project(DataDir + "CopyToProjectEmpty.xml");
File.Copy(DataDir + "CopyToProjectEmpty.mpp", OutDir + "ProjectCopying_out.mpp", true);

var mppProject = new Project(OutDir + "ProjectCopying_out.mpp");

// παραλείψτε την αντιγραφή των δεδομένων προβολής κατά την αντιγραφή κοινών δεδομένων έργου.
var copyToOptions = new CopyToOptions();
copyToOptions.CopyViewData = false;
project.CopyTo(mppProject, copyToOptions);
```

### Δείτε επίσης

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


