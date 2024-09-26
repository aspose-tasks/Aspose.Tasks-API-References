---
title: PdfSaveOptions.Pages
second_title: Aspose.Tasks for .NET API Reference
description: PdfSaveOptions property. Gets or sets the list of pages numbers to save when saving project layout to separate files. All pages will be saved if this list is empty
type: docs
weight: 60
url: /net/aspose.tasks.saving/pdfsaveoptions/pages/
---
## PdfSaveOptions.Pages property

Gets or sets the list of pages numbers to save when saving project layout to separate files. All pages will be saved if this list is empty.

```csharp
public List<int> Pages { get; set; }
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


