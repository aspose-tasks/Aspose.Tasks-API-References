---
title: "Enum TiffCompression"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.Saving.TiffCompression enum. Geeft aan welk type compressie moet worden toegepast bij het opslaan van pagina's in het TIFF-formaat."
type: docs
weight: 2250
url: /nl/net/aspose.tasks.saving/tiffcompression/
---
## TiffCompression enumeration

Bepaalt welk type compressie moet worden toegepast bij het opslaan van pagina's naar het TIFF-formaat.

```csharp
public enum TiffCompression
```

### Waarden

| Naam | Waarde | Beschrijving |
| --- | --- | --- |
| None | `1` | Geeft geen compressie aan. |
| Rle | `2` | Geeft het RLE-compressieschema aan. |
| Ccitt3 | `3` | Geeft het CCITT3-compressieschema aan. |
| Ccitt4 | `4` | Geeft het CCITT4-compressieschema aan. |
| Lzw | `5` | Geeft het LZW-compressieschema aan. |

## Voorbeelden

Toont hoe te renderen in TIFF-formaat met behulp van de RLE-compressiemodus.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var options = new ImageSaveOptions(SaveFileFormat.Tiff);

// Sla het project op met Rle-compressie
options.TiffCompression = TiffCompression.Rle;
project.Save(OutDir + "RenderMultipageTIFF_comp_rle_out.tif", options);
```

### Zie ook

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


