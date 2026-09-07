---
title: "ImageSaveOptions.HorizontalResolution"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà ImageSaveOptions. Ottiene o imposta la risoluzione orizzontale in dpi"
type: docs
weight: 30
url: /it/net/aspose.tasks.saving/imagesaveoptions/horizontalresolution/
---
## ImageSaveOptions.HorizontalResolution property

Ottiene o imposta la risoluzione orizzontale in dpi.

```csharp
public float HorizontalResolution { get; set; }
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


