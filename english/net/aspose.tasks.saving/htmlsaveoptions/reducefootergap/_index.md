---
title: HtmlSaveOptions.ReduceFooterGap
second_title: Aspose.Tasks for .NET API Reference
description: HtmlSaveOptions property. Gets or sets a value indicating whether a gap between last task and the footer must be reduced
type: docs
weight: 150
url: /net/aspose.tasks.saving/htmlsaveoptions/reducefootergap/
---
## HtmlSaveOptions.ReduceFooterGap property

Gets or sets a value indicating whether a gap between last task and the footer must be reduced.

```csharp
public bool ReduceFooterGap { get; set; }
```

## Examples

Shows how to set a value indicating whether a gap between last task and the footer must be reduced in HTML output files.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new HtmlSaveOptions
                  {
                      ReduceFooterGap = true,
                      IncludeProjectNameInPageHeader = false,
                      IncludeProjectNameInTitle = false,
                      PageSize = PageSize.A0,
                      Timescale = Timescale.Days
                  };
project.Save(OutDir + "ReducingGapBetweenTasksListAndFooter_out.html", options);
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../htmlsaveoptions/)
* assembly [Aspose.Tasks](../../../)


