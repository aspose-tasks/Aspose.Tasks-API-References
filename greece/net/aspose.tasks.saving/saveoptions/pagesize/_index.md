---
title: "SaveOptions.PageSize"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα SaveOptions. Λαμβάνει ή ορίζει το μέγεθος της σελίδας που θα αποδοθεί. Η προεπιλεγμένη τιμή είναι PageSize.A4."
type: docs
weight: 130
url: /el/net/aspose.tasks.saving/saveoptions/pagesize/
---
## SaveOptions.PageSize property

Αποκτά ή ορίζει το μέγεθος της σελίδας που θα αποδοθεί (Η προεπιλεγμένη τιμή είναι PageSize.A4).

```csharp
public PageSize PageSize { get; set; }
```

## Παραδείγματα

Δείχνει πώς να ορίσετε το μέγεθος της σελίδας (μπορεί να είναι μία από τις τιμές της απαρίθμησης &lt;see cref="P:Aspose.Tasks.Visualization.TiffCompression" /&gt;).

```csharp
var project = new Project(DataDir + "Project2.mpp");

const PresentationFormat format = PresentationFormat.GanttChart;

// Αποδώστε το έργο σε όλα τα προ-ορισμένα μεγέθη σελίδας.
foreach (var pageSize in (PageSize[])Enum.GetValues(typeof(PageSize)))
{
    var options = new PdfSaveOptions
    {
        PresentationFormat = format,
        FitContent = true,
        PageSize = pageSize
    };
    project.Save(OutDir + "PredefinedPageSizes_" + format + "_" + pageSize + "_out.pdf", options);
}
```

### Δείτε επίσης

* enum [PageSize](../../../aspose.tasks.visualization/pagesize/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


