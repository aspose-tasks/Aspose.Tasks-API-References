---
title: XpsOptions.RenderMetafileAsBitmap
second_title: Aspose.Tasks for .NET API Reference
description: XpsOptions property. Gets or sets a value indicating whether a metafile should be rendered as bitmap
type: docs
weight: 20
url: /net/aspose.tasks.saving/xpsoptions/rendermetafileasbitmap/
---
## XpsOptions.RenderMetafileAsBitmap property

Gets or sets a value indicating whether a metafile should be rendered as bitmap.

```csharp
public bool RenderMetafileAsBitmap { get; set; }
```

## Examples

Shows how to save project as XPS file.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// create XPS save options and tune the parameters
var options = new XpsOptions
{
    RenderMetafileAsBitmap = true
};

project.Save(OutDir + "UseSvgOptions_out.xps", options);
```

### See Also

* class [XpsOptions](../)
* namespace [Aspose.Tasks.Saving](../../xpsoptions/)
* assembly [Aspose.Tasks](../../../)


