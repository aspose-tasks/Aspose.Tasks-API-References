---
title: "SaveOptions.CustomPageSize"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα SaveOptions. Λαμβάνει ή ορίζει το προσαρμοσμένο μέγεθος σελίδας σε μονάδες points, 1 point = 1/72 ίντσας."
type: docs
weight: 20
url: /el/net/aspose.tasks.saving/saveoptions/custompagesize/
---
## SaveOptions.CustomPageSize property

Αποκτά ή ορίζει το προσαρμοσμένο μέγεθος σελίδας σε points (1 point = 1/72 ίντσας).

```csharp
public SizeF CustomPageSize { get; set; }
```

## Παραδείγματα

Δείχνει πώς να ορίσετε προσαρμοσμένο μέγεθος σελίδας όταν το έργο αποθηκεύεται σε PDF.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions();
options.PresentationFormat = PresentationFormat.GanttChart;
options.CustomPageSize = new SizeF(5.8F * 72, 8.3F * 72);

project.Save(OutDir + "WorkWithCustomPageSize_out.pdf", options);
```

### Δείτε επίσης

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


