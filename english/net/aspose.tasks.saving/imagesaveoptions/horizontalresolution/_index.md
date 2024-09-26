---
title: ImageSaveOptions.HorizontalResolution
second_title: Aspose.Tasks for .NET API Reference
description: ImageSaveOptions property. Gets or sets the horizontal resolution in dpi
type: docs
weight: 30
url: /net/aspose.tasks.saving/imagesaveoptions/horizontalresolution/
---
## ImageSaveOptions.HorizontalResolution property

Gets or sets the horizontal resolution in dpi.

```csharp
public float HorizontalResolution { get; set; }
```

## Examples

Shows how to set pixel format which is used during conversion into image formats.

```csharp
var project = new Project(DataDir + "Project1.mpp");
var options = new ImageSaveOptions(SaveFileFormat.Tiff);
options.HorizontalResolution = 72;
options.VerticalResolution = 72;
options.PixelFormat = PixelFormat.Format24bppRgb;
project.Save(OutDir + "RenderProjectDataToFormat24bppRgb_out.tif", options);
```

### See Also

* class [ImageSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../imagesaveoptions/)
* assembly [Aspose.Tasks](../../../)


