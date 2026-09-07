---
title: "Enum TiffCompression"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Enum Aspose.Tasks.Saving.TiffCompression. Specifica quale tipo di compressione applicare quando si salvano le pagine nel formato TIFF"
type: docs
weight: 2250
url: /it/net/aspose.tasks.saving/tiffcompression/
---
## TiffCompression enumeration

Specifica quale tipo di compressione applicare quando si salvano le pagine nel formato TIFF.

```csharp
public enum TiffCompression
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| None | `1` | Specifica nessuna compressione. |
| Rle | `2` | Specifica lo schema di compressione RLE. |
| Ccitt3 | `3` | Specifica lo schema di compressione CCITT3. |
| Ccitt4 | `4` | Specifica lo schema di compressione CCITT4. |
| Lzw | `5` | Specifica lo schema di compressione LZW. |

## Esempi

Mostra come rendere in formato TIFF utilizzando la modalità di compressione RLE.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var options = new ImageSaveOptions(SaveFileFormat.Tiff);

// Salva il progetto con compressione RLE
options.TiffCompression = TiffCompression.Rle;
project.Save(OutDir + "RenderMultipageTIFF_comp_rle_out.tif", options);
```

### Vedi anche

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


