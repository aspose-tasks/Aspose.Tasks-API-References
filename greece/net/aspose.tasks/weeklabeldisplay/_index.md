---
title: "Enum WeekLabelDisplay"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.WeekLabelDisplay enum. Καθορίζει πώς εμφανίζεται η ετικέτα εβδομάδας"
type: docs
weight: 3560
url: /el/net/aspose.tasks/weeklabeldisplay/
---
## WeekLabelDisplay enumeration

Καθορίζει πώς εμφανίζεται η ετικέτα εβδομάδας.

```csharp
public enum WeekLabelDisplay
```

### Τιμές

| Όνομα | Τιμή | Περιγραφή |
| --- | --- | --- |
| W | `0` | \"w\" ετικέτα. |
| Wk | `1` | \"wk\" ετικέτα. |
| Week | `2` | \"week\" ετικέτα. |

## Παραδείγματα

Δείχνει πώς να ορίσετε την ετικέτα εβδομάδας των επιλογών εμφάνισης του έργου (περίπτωση 1).

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// ...
// ορίστε πώς εμφανίζεται η ετικέτα εβδομάδας
project.DisplayOptions.WeekLabel = WeekLabelDisplay.W;

// ...
```

### Δείτε επίσης

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


