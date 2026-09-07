---
title: "ImageSaveOptions.TiffCompression"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà ImageSaveOptions. Ottiene o imposta il tipo di compressione da applicare quando si salvano le immagini generate nel formato TIFF"
type: docs
weight: 90
url: /it/net/aspose.tasks.saving/imagesaveoptions/tiffcompression/
---
## ImageSaveOptions.TiffCompression property

Ottiene o imposta il tipo di compressione da applicare quando le immagini generate vengono salvate nel formato TIFF.

```csharp
public TiffCompression TiffCompression { get; set; }
```

## Osservazioni

Ha effetto solo quando si salva in TIFF. Il valore predefinito è `LZW`.

## Esempi

Mostra come impostare la compressione TIFF dei file TIFF di output.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// Per manipolare la compressione TIFF possiamo usare la proprietà ImageSaveOptions.TiffCompression.
var options = new ImageSaveOptions(SaveFileFormat.Tiff)
{
    TiffCompression = TiffCompression.Lzw
};

project.Save(OutDir + "SaveProjectAsTiff_out.tif", options);
```

### Vedi anche

* enum [TiffCompression](../../tiffcompression/)
* class [ImageSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../imagesaveoptions/)
* assembly [Aspose.Tasks](../../../)


