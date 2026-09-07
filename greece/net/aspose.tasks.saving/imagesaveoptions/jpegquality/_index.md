---
title: "ImageSaveOptions.JpegQuality"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα ImageSaveOptions. Λαμβάνει ή ορίζει την ποιότητα JPEG. Η επιτρεπόμενη περιοχή τιμών είναι 0..100"
type: docs
weight: 40
url: /el/net/aspose.tasks.saving/imagesaveoptions/jpegquality/
---
## ImageSaveOptions.JpegQuality property

Λαμβάνει ή ορίζει την ποιότητα JPEG. Η επιτρεπόμενη περιοχή τιμών είναι 0..100.

```csharp
public int JpegQuality { get; set; }
```

## Παραδείγματα

Δείχνει πώς να ορίσετε την ποιότητα JPEG των εξαγόμενων αρχείων JPEG.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

// Για να χειριστείτε την ποιότητα JPEG, μπορείτε να χρησιμοποιήσετε την ιδιότητα ImageSaveOptions.JpegQuality.
// Το επιτρεπόμενο εύρος τιμών είναι 0..100.
var options = new ImageSaveOptions(SaveFileFormat.Jpeg)
{
    JpegQuality = 50
};

project.Save(OutDir + "SaveProjectAsJPEG_out.jpeg", options);
```

### Δείτε επίσης

* class [ImageSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../imagesaveoptions/)
* assembly [Aspose.Tasks](../../../)


