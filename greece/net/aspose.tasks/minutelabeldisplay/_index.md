---
title: "Απαρίθμηση MinuteLabelDisplay"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Απαρίθμηση Aspose.Tasks.MinuteLabelDisplay. Καθορίζει πώς εμφανίζεται η ετικέτα λεπτών."
type: docs
weight: 1030
url: /el/net/aspose.tasks/minutelabeldisplay/
---
## MinuteLabelDisplay enumeration

Καθορίζει πώς εμφανίζεται η ετικέτα λεπτών.

```csharp
public enum MinuteLabelDisplay
```

### Τιμές

| Όνομα | Τιμή | Περιγραφή |
| --- | --- | --- |
| M | `0` | Ορίζει τη λίστα Minutes στο MS Project ως m. |
| Min | `1` | Ορίζει τη λίστα Minutes στο MS Project ως min. |
| Minute | `2` | Ορίζει τη λίστα Minutes στο MS Project ως minute. |

## Παραδείγματα

Δείχνει πώς να ορίσετε την ετικέτα λεπτών των επιλογών εμφάνισης του έργου (περίπτωση 1).

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// ...
// ορίστε πώς εμφανίζεται η ετικέτα λεπτών
project.DisplayOptions.MinuteLabel = MinuteLabelDisplay.M;

// ...
```

### Δείτε επίσης

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


