---
title: PdfSaveOptions.PdfSaveOptions
second_title: Aspose.Tasks for .NET API Reference
description: PdfSaveOptions constructor. Initializes a new instance of the PdfSaveOptions class that can be used to save a document in the PDF format
type: docs
weight: 10
url: /net/aspose.tasks.saving/pdfsaveoptions/pdfsaveoptions/
---
## PdfSaveOptions constructor

Initializes a new instance of the [`PdfSaveOptions`](../) class that can be used to save a document in the [`PDF`](../../savefileformat/) format.

```csharp
public PdfSaveOptions()
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

* class [PdfSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../pdfsaveoptions/)
* assembly [Aspose.Tasks](../../../)


