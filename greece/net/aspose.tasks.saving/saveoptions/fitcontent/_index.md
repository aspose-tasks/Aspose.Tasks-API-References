---
title: "SaveOptions.FitContent"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα SaveOptions. Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν το ύψος της γραμμής πρέπει να αυξηθεί ώστε να ταιριάζει στο περιεχόμενό της"
type: docs
weight: 50
url: /el/net/aspose.tasks.saving/saveoptions/fitcontent/
---
## SaveOptions.FitContent property

Αποκτά ή ορίζει μια τιμή που υποδεικνύει εάν το ύψος της γραμμής πρέπει να αυξηθεί ώστε να ταιριάζει στο περιεχόμενό της.

```csharp
public bool FitContent { get; set; }
```

## Παραδείγματα

Δείχνει πώς να ορίσετε την επιλογή εάν το ύψος της γραμμής πρέπει να αυξηθεί ώστε να ταιριάζει στο περιεχόμενό της.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
SaveOptions options = new PdfSaveOptions
{
    // Ορίστε την επιλογή fit content σε true
    FitContent = true,
    Timescale = Timescale.Months,
    PresentationFormat = PresentationFormat.TaskUsage
};
project.Save(OutDir + "FitContentsToCellSize_out.pdf", options);
```

### Δείτε επίσης

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


