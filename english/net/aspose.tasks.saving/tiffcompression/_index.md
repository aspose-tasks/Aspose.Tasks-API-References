---
title: Enum TiffCompression
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.Saving.TiffCompression enum. Specifies what type of compression to apply when saving pages to the TIFF format
type: docs
weight: 2180
url: /net/aspose.tasks.saving/tiffcompression/
---
## TiffCompression enumeration

Specifies what type of compression to apply when saving pages to the TIFF format.

```csharp
public enum TiffCompression
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| None | `1` | Specifies no compression. |
| Rle | `2` | Specifies the RLE compression scheme. |
| Ccitt3 | `3` | Specifies the CCITT3 compression scheme. |
| Ccitt4 | `4` | Specifies the CCITT4 compression scheme. |
| Lzw | `5` | Specifies the LZW compression scheme. |

## Examples

Shows how to render in TIFF format by using RLE compression mode.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var options = new ImageSaveOptions(SaveFileFormat.Tiff);

// Save the project with Rle compression
options.TiffCompression = TiffCompression.Rle;
project.Save(OutDir + "RenderMultipageTIFF_comp_rle_out.tif", options);
```

### See Also

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


