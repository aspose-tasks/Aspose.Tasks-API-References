---
title: XpsOptions.XpsOptions
second_title: Aspose.Tasks for .NET API Reference
description: XpsOptions constructor. Initializes a new instance of the XpsOptions class
type: docs
weight: 10
url: /net/aspose.tasks.saving/xpsoptions/xpsoptions/
---
## XpsOptions constructor

Initializes a new instance of the [`XpsOptions`](../) class.

```csharp
public XpsOptions()
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


