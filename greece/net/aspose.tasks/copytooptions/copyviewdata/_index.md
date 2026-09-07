---
title: "CopyToOptions.CopyViewData"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα CopyToOptions. Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν θα αντιγραφούν δεδομένα προβολής κατά την αντιγραφή δεδομένων έργου. Η προεπιλεγμένη τιμή είναι true"
type: docs
weight: 20
url: /el/net/aspose.tasks/copytooptions/copyviewdata/
---
## CopyToOptions.CopyViewData property

Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει αν θα αντιγραφούν τα δεδομένα προβολής κατά την αντιγραφή δεδομένων έργου. Η προεπιλεγμένη τιμή είναι true.

```csharp
public bool CopyViewData { get; set; }
```

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

* class [CopyToOptions](../)
* namespace [Aspose.Tasks](../../copytooptions/)
* assembly [Aspose.Tasks](../../../)


