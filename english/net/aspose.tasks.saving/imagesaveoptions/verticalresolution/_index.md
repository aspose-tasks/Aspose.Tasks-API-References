---
title: ImageSaveOptions.VerticalResolution
second_title: Aspose.Tasks for .NET API Reference
description: ImageSaveOptions property. Gets or sets the vertical resolution in dpi
type: docs
weight: 100
url: /net/aspose.tasks.saving/imagesaveoptions/verticalresolution/
---
## ImageSaveOptions.VerticalResolution property

Gets or sets the vertical resolution in dpi.

```csharp
public float VerticalResolution { get; set; }
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


