---
title: "ImageSaveOptions.JpegQuality"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "ImageSaveOptions eigenschap. Haalt de JPEG‑kwaliteit op of stelt deze in. Het toegestane waardebereik is 0..100"
type: docs
weight: 40
url: /nl/net/aspose.tasks.saving/imagesaveoptions/jpegquality/
---
## ImageSaveOptions.JpegQuality property

Haalt op of stelt een JPEG‑kwaliteit in. Het toegestane waardebereik is 0..100.

```csharp
public int JpegQuality { get; set; }
```

## Voorbeelden

Toont hoe de JPEG-kwaliteit van uitvoer‑JPEG‑bestanden in te stellen.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

// Om de JPEG-kwaliteit te manipuleren kan men de eigenschap ImageSaveOptions.JpegQuality gebruiken.
// Het toegestane waardebereik is 0..100.
var options = new ImageSaveOptions(SaveFileFormat.Jpeg)
{
    JpegQuality = 50
};

project.Save(OutDir + "SaveProjectAsJPEG_out.jpeg", options);
```

### Zie ook

* class [ImageSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../imagesaveoptions/)
* assembly [Aspose.Tasks](../../../)


