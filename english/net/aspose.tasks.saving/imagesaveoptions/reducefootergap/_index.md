---
title: ImageSaveOptions.ReduceFooterGap
second_title: Aspose.Tasks for .NET API Reference
description: ImageSaveOptions property. Gets or sets a value indicating whether a gap between last task and the footer must be reduced
type: docs
weight: 80
url: /net/aspose.tasks.saving/imagesaveoptions/reducefootergap/
---
## ImageSaveOptions.ReduceFooterGap property

Gets or sets a value indicating whether a gap between last task and the footer must be reduced.

```csharp
public bool ReduceFooterGap { get; set; }
```

## Examples

Shows how to set a value indicating whether a gap between last task and the footer must be reduced.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

// Use ReduceFooterGap property to reduce the gap between list of tasks and Footer
var imageSaveOptions = new ImageSaveOptions(SaveFileFormat.Png)
                           {
                               ReduceFooterGap = true, /* set to true */ 
                               RenderToSinglePage = false,
                               PageSize = PageSize.A0,
                               Timescale = Timescale.Days
                           };
project.Save(OutDir + "ReducingGapBetweenTasksListAndFooter_out.png", imageSaveOptions);
```

### See Also

* class [ImageSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../imagesaveoptions/)
* assembly [Aspose.Tasks](../../../)


