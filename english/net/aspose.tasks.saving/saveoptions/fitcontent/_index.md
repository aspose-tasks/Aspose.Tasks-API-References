---
title: SaveOptions.FitContent
second_title: Aspose.Tasks for .NET API Reference
description: SaveOptions property. Gets or sets a value indicating whether row height should be increased to fit its content
type: docs
weight: 50
url: /net/aspose.tasks.saving/saveoptions/fitcontent/
---
## SaveOptions.FitContent property

Gets or sets a value indicating whether row height should be increased to fit its content.

```csharp
public bool FitContent { get; set; }
```

## Examples

Shows how to set the option whether row height should be increased to fit its content.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
SaveOptions options = new PdfSaveOptions
{
    // Set option fit content to true
    FitContent = true,
    Timescale = Timescale.Months,
    PresentationFormat = PresentationFormat.TaskUsage
};
project.Save(OutDir + "FitContentsToCellSize_out.pdf", options);
```

### See Also

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


