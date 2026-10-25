---
title: "MPPSaveOptions.ClearVba"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα MPPSaveOptions. Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν θα αφαιρεθούν τα υπάρχοντα δεδομένα μακροεντολών VBA κατά την αποθήκευση ενός έργου σε μορφή MPP."
type: docs
weight: 20
url: /el/net/aspose.tasks.saving/mppsaveoptions/clearvba/
---
## MPPSaveOptions.ClearVba property

Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν θα αφαιρεθούν τα υπάρχοντα δεδομένα μακροεντολών VBA κατά την αποθήκευση ενός έργου σε μορφή MPP.

```csharp
public bool ClearVba { get; set; }
```

## Παραδείγματα

Δείχνει πώς να αφαιρέσετε μακροεντολές VBA από αρχείο MPP.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");
project.Save(OutDir + "Vba.cleared.mpp", new MPPSaveOptions() { ClearVba = true });
```

### Δείτε επίσης

* class [MPPSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../mppsaveoptions/)
* assembly [Aspose.Tasks](../../../)


