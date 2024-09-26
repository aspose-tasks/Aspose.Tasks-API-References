---
title: ImageSaveOptions.JpegQuality
second_title: Aspose.Tasks for .NET API Reference
description: ImageSaveOptions property. Gets or sets a JPEG quality. The allowed value range is 0..100
type: docs
weight: 40
url: /net/aspose.tasks.saving/imagesaveoptions/jpegquality/
---
## ImageSaveOptions.JpegQuality property

Gets or sets a JPEG quality. The allowed value range is 0..100.

```csharp
public int JpegQuality { get; set; }
```

## Examples

Shows how to set JPEG quality of output JPEG files.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

// in order to manipulate JPEG quality one can use ImageSaveOptions.JpegQuality property.
// The allowed value range is 0..100.
var options = new ImageSaveOptions(SaveFileFormat.Jpeg)
{
    JpegQuality = 50
};

project.Save(OutDir + "SaveProjectAsJPEG_out.jpeg", options);
```

### See Also

* class [ImageSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../imagesaveoptions/)
* assembly [Aspose.Tasks](../../../)


