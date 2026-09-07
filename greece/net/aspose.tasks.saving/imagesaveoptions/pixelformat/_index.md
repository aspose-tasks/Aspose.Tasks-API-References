---
title: "ImageSaveOptions.PixelFormat"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα ImageSaveOptions. Λαμβάνει ή ορίζει τη μορφή των δεδομένων χρώματος για κάθε pixel στην εικόνα."
type: docs
weight: 70
url: /el/net/aspose.tasks.saving/imagesaveoptions/pixelformat/
---
## ImageSaveOptions.PixelFormat property

Λαμβάνει ή ορίζει τη μορφή των χρωματικών δεδομένων για κάθε pixel στην εικόνα.

```csharp
public PixelFormat PixelFormat { get; set; }
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


