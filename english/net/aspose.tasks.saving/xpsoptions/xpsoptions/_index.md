---
title: XpsOptions
second_title: Aspose.Tasks for .NET API Reference
description: Initializes a new instance of the XpsOptionsaspose.tasks.saving/xpsoptions class.
type: docs
weight: 10
url: /net/aspose.tasks.saving/xpsoptions/xpsoptions/
---
## XpsOptions constructor

Initializes a new instance of the [`XpsOptions`](../../xpsoptions) class.

```csharp
public XpsOptions()
```

### Examples

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

* class [XpsOptions](../../xpsoptions)
* namespace [Aspose.Tasks.Saving](../../xpsoptions)
* assembly [Aspose.Tasks](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
