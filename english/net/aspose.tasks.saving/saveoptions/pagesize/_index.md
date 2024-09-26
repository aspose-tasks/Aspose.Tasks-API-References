---
title: SaveOptions.PageSize
second_title: Aspose.Tasks for .NET API Reference
description: SaveOptions property. Gets or sets the size of page to be rendered Default value is PageSize.A4
type: docs
weight: 130
url: /net/aspose.tasks.saving/saveoptions/pagesize/
---
## SaveOptions.PageSize property

Gets or sets the size of page to be rendered (Default value is PageSize.A4).

```csharp
public PageSize PageSize { get; set; }
```

## Examples

Shows how to set page size (can be one of the values of the &lt;see cref="P:Aspose.Tasks.Visualization.TiffCompression" /&gt; enumeration).

```csharp
var project = new Project(DataDir + "Project2.mpp");

const PresentationFormat format = PresentationFormat.GanttChart;

// Render the project to all Pre-Defined page sizes
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

### See Also

* enum [PageSize](../../../aspose.tasks.visualization/pagesize/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


