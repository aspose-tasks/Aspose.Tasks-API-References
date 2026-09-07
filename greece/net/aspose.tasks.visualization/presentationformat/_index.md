---
title: "Απαρίθμηση PresentationFormat"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.Visualization.PresentationFormat enum. Απαρίθμηση για μορφή παρουσίασης"
type: docs
weight: 3270
url: /el/net/aspose.tasks.visualization/presentationformat/
---
## PresentationFormat enumeration

Απαρίθμηση για μορφή παρουσίασης.

```csharp
public enum PresentationFormat
```

### Τιμές

| Όνομα | Τιμή | Περιγραφή |
| --- | --- | --- |
| GanttChart | `0` | Μορφή παρουσίασης του Gantt Chart. |
| TaskUsage | `1` | Μορφή παρουσίασης χρήσης εργασίας. |
| ResourceUsage | `2` | Μορφή παρουσίασης χρήσης πόρων. |
| ResourceSheet | `3` | Μορφή παρουσίασης φύλλου πόρων. |
| TaskSheet | `4` | Μορφή παρουσίασης φύλλου εργασίας. |

## Παραδείγματα

Δείχνει πώς να αποδίδεται η προβολή φύλλου πόρων.

```csharp
var project = new Project(DataDir + "ResourceSheetView.mpp");

SaveOptions options = new PdfSaveOptions();

// Ορίστε τη Μορφή Παρουσίασης σε Φύλλο Πόρων
options.PresentationFormat = PresentationFormat.ResourceSheet;
project.Save(OutDir + "ResourceSheetView_out.pdf", options);
```

### Δείτε επίσης

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


