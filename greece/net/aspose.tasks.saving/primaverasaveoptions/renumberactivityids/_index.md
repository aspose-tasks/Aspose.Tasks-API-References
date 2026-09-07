---
title: "PrimaveraSaveOptions.RenumberActivityIds"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα PrimaveraSaveOptions. Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν χρειάζεται η επανααρίθμηση των αναγνωριστικών δραστηριότητας"
type: docs
weight: 50
url: /el/net/aspose.tasks.saving/primaverasaveoptions/renumberactivityids/
---
## PrimaveraSaveOptions.RenumberActivityIds property

Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν χρειάζεται η επανααρίθμηση των αναγνωριστικών δραστηριότητας.

```csharp
public bool RenumberActivityIds { get; set; }
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


