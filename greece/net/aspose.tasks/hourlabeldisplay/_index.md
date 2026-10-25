---
title: "Enum HourLabelDisplay"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.HourLabelDisplay enum. Καθορίζει πώς εμφανίζεται η ετικέτα ώρας."
type: docs
weight: 820
url: /el/net/aspose.tasks/hourlabeldisplay/
---
## HourLabelDisplay enumeration

Καθορίζει πώς εμφανίζεται η ετικέτα ώρας.

```csharp
public enum HourLabelDisplay
```

### Τιμές

| Όνομα | Τιμή | Περιγραφή |
| --- | --- | --- |
| H | `0` | \"h\" ετικέτα. |
| Hr | `1` | \"hr\" ετικέτα. |
| Hour | `2` | \"hour(s)\" ετικέτα. |

## Παραδείγματα

Δείχνει πώς να ορίσετε την ετικέτα ώρας των επιλογών εμφάνισης του έργου (περίπτωση 1).

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// ...
// ορίστε πώς εμφανίζεται η ετικέτα ώρας
project.DisplayOptions.HourLabel = HourLabelDisplay.H;

// ...
```

### Δείτε επίσης

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


