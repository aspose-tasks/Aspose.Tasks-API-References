---
title: "ImageSaveOptions.JpegQuality"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà ImageSaveOptions. Ottiene o imposta la qualità JPEG. L'intervallo di valori consentito è 0..100"
type: docs
weight: 40
url: /it/net/aspose.tasks.saving/imagesaveoptions/jpegquality/
---
## ImageSaveOptions.JpegQuality property

Ottiene o imposta la qualità JPEG. L'intervallo di valori consentito è 0..100.

```csharp
public int JpegQuality { get; set; }
```

## Esempi

Mostra come impostare la qualità JPEG dei file JPEG di output.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

// Per manipolare la qualità JPEG è possibile utilizzare la proprietà ImageSaveOptions.JpegQuality.
// L'intervallo di valori consentito è 0..100.
var options = new ImageSaveOptions(SaveFileFormat.Jpeg)
{
    JpegQuality = 50
};

project.Save(OutDir + "SaveProjectAsJPEG_out.jpeg", options);
```

### Vedi anche

* class [ImageSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../imagesaveoptions/)
* assembly [Aspose.Tasks](../../../)


