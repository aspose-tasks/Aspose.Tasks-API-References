---
title: ImageSaveOptions.TiffCompression
second_title: Aspose.Tasks for .NET API Reference
description: ImageSaveOptions property. Gets or sets the type of compression to apply when saving generated images to the TIFF format
type: docs
weight: 90
url: /net/aspose.tasks.saving/imagesaveoptions/tiffcompression/
---
## ImageSaveOptions.TiffCompression property

Gets or sets the type of compression to apply when saving generated images to the TIFF format.

```csharp
public TiffCompression TiffCompression { get; set; }
```

## Remarks

Has effect only when saving to TIFF. The default value is `LZW`.

## Examples

Shows how to set TIFF compression of the output TIFF files.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// in order to manipulate TIFF compression we can use ImageSaveOptions.TiffCompression property.
var options = new ImageSaveOptions(SaveFileFormat.Tiff)
{
    TiffCompression = TiffCompression.Lzw
};

project.Save(OutDir + "SaveProjectAsTiff_out.tif", options);
```

### See Also

* enum [TiffCompression](../../tiffcompression/)
* class [ImageSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../imagesaveoptions/)
* assembly [Aspose.Tasks](../../../)


