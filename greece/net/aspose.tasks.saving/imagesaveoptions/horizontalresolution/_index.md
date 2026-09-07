---
title: "ImageSaveOptions.HorizontalResolution"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα ImageSaveOptions. Λαμβάνει ή ορίζει την οριζόντια ανάλυση σε dpi"
type: docs
weight: 30
url: /el/net/aspose.tasks.saving/imagesaveoptions/horizontalresolution/
---
## ImageSaveOptions.HorizontalResolution property

Λαμβάνει ή ορίζει την οριζόντια ανάλυση σε dpi.

```csharp
public float HorizontalResolution { get; set; }
```

## Παραδείγματα

Δείχνει πώς να ορίσετε τη μορφή pixel που χρησιμοποιείται κατά τη μετατροπή σε μορφές εικόνας.

```csharp
var project = new Project(DataDir + "Project1.mpp");
var options = new ImageSaveOptions(SaveFileFormat.Tiff);
options.HorizontalResolution = 72;
options.VerticalResolution = 72;
options.PixelFormat = PixelFormat.Format24bppRgb;
project.Save(OutDir + "RenderProjectDataToFormat24bppRgb_out.tif", options);
```

### Δείτε επίσης

* class [ImageSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../imagesaveoptions/)
* assembly [Aspose.Tasks](../../../)


