---
title: "PrimaveraSaveOptions.PrimaveraSaveOptions"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κατασκευαστής PrimaveraSaveOptions. Αρχικοποιεί μια νέα παρουσία της κλάσης PrimaveraSaveOptions"
type: docs
weight: 10
url: /el/net/aspose.tasks.saving/primaverasaveoptions/primaverasaveoptions/
---
## PrimaveraSaveOptions constructor

Αρχικοποιεί μια νέα παρουσία της κλάσης [`PrimaveraSaveOptions`](../).

```csharp
public PrimaveraSaveOptions()
```

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

* class [PrimaveraSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../primaverasaveoptions/)
* assembly [Aspose.Tasks](../../../)


