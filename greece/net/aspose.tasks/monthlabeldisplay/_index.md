---
title: "Enum MonthLabelDisplay"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.MonthLabelDisplay enum. Καθορίζει πώς εμφανίζεται η ετικέτα του μήνα"
type: docs
weight: 1060
url: /el/net/aspose.tasks/monthlabeldisplay/
---
## MonthLabelDisplay enumeration

Καθορίζει πώς εμφανίζεται η ετικέτα μήνα.

```csharp
public enum MonthLabelDisplay
```

### Τιμές

| Όνομα | Τιμή | Περιγραφή |
| --- | --- | --- |
| Mo | `0` | Ορίζει τη λίστα Μήνες στο MS Project ως mo. |
| Mon | `1` | Ορίζει τη λίστα Μήνες στο MS Project ως mon. |
| Month | `2` | Ορίζει τη λίστα Μήνες στο MS Project ως month. |

## Παραδείγματα

Δείχνει πώς να ορίσετε την ετικέτα του μήνα των επιλογών εμφάνισης του έργου (περίπτωση 1).

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// ...
// ορίστε πώς εμφανίζεται η ετικέτα του μήνα
project.DisplayOptions.MonthLabel = MonthLabelDisplay.Mo;

// ...
```

### Δείτε επίσης

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


