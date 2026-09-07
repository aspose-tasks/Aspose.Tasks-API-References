---
title: "Enum DayLabelDisplay"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.DayLabelDisplay enum. Καθορίζει πώς εμφανίζεται η ετικέτα ημέρας"
type: docs
weight: 440
url: /el/net/aspose.tasks/daylabeldisplay/
---
## DayLabelDisplay enumeration

Καθορίζει πώς εμφανίζεται η ετικέτα ημέρας.

```csharp
public enum DayLabelDisplay
```

### Τιμές

| Όνομα | Τιμή | Περιγραφή |
| --- | --- | --- |
| D | `0` | Ορίζει τη λίστα Ημερών στο MS Project ως d. |
| Dy | `1` | Ορίζει τη λίστα Ημερών στο MS Project ως dy. |
| Day | `2` | Ορίζει τη λίστα Ημερών στο MS Project ως day. |

## Παραδείγματα

Δείχνει πώς να ορίσετε την ετικέτα ημέρας των επιλογών εμφάνισης του έργου (περίπτωση 1).

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// ...
// ορίστε πώς εμφανίζεται η ετικέτα ημέρας
project.DisplayOptions.DayLabel = DayLabelDisplay.D;

// ...
```

### Δείτε επίσης

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


