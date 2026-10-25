---
title: "ImageSaveOptions.PixelFormat"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà ImageSaveOptions. Ottiene o imposta il formato dei dati di colore per ogni pixel nell'immagine"
type: docs
weight: 70
url: /it/net/aspose.tasks.saving/imagesaveoptions/pixelformat/
---
## ImageSaveOptions.PixelFormat property

Ottiene o imposta il formato dei dati di colore per ogni pixel nell'immagine.

```csharp
public PixelFormat PixelFormat { get; set; }
```

## Esempi

Mostra come impostare il formato pixel utilizzato durante la conversione in formati immagine.

```csharp
var project = new Project(DataDir + "Project1.mpp");
var options = new ImageSaveOptions(SaveFileFormat.Tiff);
options.HorizontalResolution = 72;
options.VerticalResolution = 72;
options.PixelFormat = PixelFormat.Format24bppRgb;
project.Save(OutDir + "RenderProjectDataToFormat24bppRgb_out.tif", options);
```

### Vedi anche

* class [ImageSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../imagesaveoptions/)
* assembly [Aspose.Tasks](../../../)


