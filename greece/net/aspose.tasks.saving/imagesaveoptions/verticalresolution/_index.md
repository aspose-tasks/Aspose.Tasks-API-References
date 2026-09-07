---
title: "ImageSaveOptions.VerticalResolution"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα ImageSaveOptions. Λαμβάνει ή ορίζει την κάθετη ανάλυση σε dpi."
type: docs
weight: 100
url: /el/net/aspose.tasks.saving/imagesaveoptions/verticalresolution/
---
## ImageSaveOptions.VerticalResolution property

Λαμβάνει ή ορίζει την κάθετη ανάλυση σε dpi.

```csharp
public float VerticalResolution { get; set; }
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


