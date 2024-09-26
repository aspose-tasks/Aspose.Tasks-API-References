---
title: ImageSaveOptions.ImageSaveOptions
second_title: Aspose.Tasks for .NET API Reference
description: ImageSaveOptions constructor. Initializes a new instance of the ImageSaveOptions class which can be used to save rendered images in TIFF PNG BMP or JPEG formats
type: docs
weight: 10
url: /net/aspose.tasks.saving/imagesaveoptions/imagesaveoptions/
---
## ImageSaveOptions constructor

Initializes a new instance of the [`ImageSaveOptions`](../) class which can be used to save rendered images in TIFF, PNG, BMP or JPEG formats.

```csharp
public ImageSaveOptions(SaveFileFormat saveFormat)
```

| Parameter | Type | Description |
| --- | --- | --- |
| saveFormat | SaveFileFormat | Can be TIFF, PNG, BMP or JPEG[`SaveFileFormat`](../../savefileformat/). |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentException | Thrown of *saveFormat* is not a valid image format. The valid values are TIFF, PNG, BMP or JPEG. |

## Examples

Shows how to save project into a stream as an image.

```csharp
var project = new Project();

using (var stream = new FileStream(OutDir + "EmptyProjectSaveStream_out.xml", FileMode.Create, FileAccess.Write))
{
    var options = new ImageSaveOptions(SaveFileFormat.Png);

    // by using of ImageSaveOptions we save the project into image format
    project.Save(stream, options);
}
```

### See Also

* enum [SaveFileFormat](../../savefileformat/)
* class [ImageSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../imagesaveoptions/)
* assembly [Aspose.Tasks](../../../)


