---
title: SaveOptions.PageCount
second_title: Aspose.Tasks for .NET API Reference
description: SaveOptions property. Gets or sets the number of pages of project
type: docs
weight: 120
url: /net/aspose.tasks.saving/saveoptions/pagecount/
---
## SaveOptions.PageCount property

Gets or sets the number of pages of project.

```csharp
public int PageCount { get; }
```

## Examples

Shows how to save selected pages of a project into PDF file.

```csharp
var project = new Project(DataDir + "Software Development Plan.mpp");
var options = new PdfSaveOptions();
options.RenderToSinglePage = false;
options.Pages = new List<int>();

// lets check the number of pages can be exported
Console.WriteLine("Page Count: " + options.PageCount);

options.Pages.Add(1);
options.Pages.Add(4);
project.Save(OutDir + "SaveToMultiplePDFFiles_out.pdf", options);
```

### See Also

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


