---
title: "Απαρίθμηση YearLabelDisplay"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Απαρίθμηση Aspose.Tasks.YearLabelDisplay. Καθορίζει πώς εμφανίζεται η ετικέτα του έτους."
type: docs
weight: 3680
url: /el/net/aspose.tasks/yearlabeldisplay/
---
## YearLabelDisplay enumeration

Καθορίζει πώς εμφανίζεται η ετικέτα έτους.

```csharp
public enum YearLabelDisplay
```

### Τιμές

| Όνομα | Τιμή | Περιγραφή |
| --- | --- | --- |
| Y | `0` | Ορίζει τη λίστα Ετών στο MS Project ως mo. |
| Yr | `1` | Ορίζει τη λίστα Ετών στο MS Project ως mon. |
| Year | `2` | Ορίζει τη λίστα Ετών στο MS Project ως μήνα. |

## Παραδείγματα

Δείχνει πώς να ορίσετε την ετικέτα έτους των επιλογών εμφάνισης του έργου (περίπτωση 1).

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// ...
// ορίστε πώς εμφανίζεται η ετικέτα έτους
project.DisplayOptions.YearLabel = YearLabelDisplay.Y;

// ...
```

### Δείτε επίσης

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


