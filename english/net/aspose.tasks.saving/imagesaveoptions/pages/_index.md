---
title: ImageSaveOptions.Pages
second_title: Aspose.Tasks for .NET API Reference
description: ImageSaveOptions property. Gets or sets a list of page numbers to save when saving project layout to separate files. All pages will be saved if this list is empty
type: docs
weight: 50
url: /net/aspose.tasks.saving/imagesaveoptions/pages/
---
## ImageSaveOptions.Pages property

Gets or sets a list of page numbers to save when saving project layout to separate files. All pages will be saved if this list is empty.

```csharp
public List<int> Pages { get; set; }
```

## Examples

Shows how to save selected pages in as an image.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new ImageSaveOptions(SaveFileFormat.Jpeg)
                  {
                      RenderToSinglePage = false,
                      StartDate = project.Get(Prj.StartDate),
                      EndDate = project.Get(Prj.FinishDate),
                      PageSize = PageSize.Letter
                  };
options.Pages.Add(2);

project.Save(OutDir + "SaveSelectedPagesImageSaveOptions_page2_out.jpeg", options);
```

### See Also

* class [ImageSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../imagesaveoptions/)
* assembly [Aspose.Tasks](../../../)


