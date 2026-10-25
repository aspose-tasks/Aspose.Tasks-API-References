---
title: "Enum TiffCompression"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Aspose.Tasks.Saving.TiffCompression enum. Spécifie le type de compression à appliquer lors de l'enregistrement des pages au format TIFF"
type: docs
weight: 2250
url: /fr/net/aspose.tasks.saving/tiffcompression/
---
## TiffCompression enumeration

Spécifie le type de compression à appliquer lors de l'enregistrement des pages au format TIFF.

```csharp
public enum TiffCompression
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| None | `1` | Spécifie aucune compression. |
| Rle | `2` | Spécifie le schéma de compression RLE. |
| Ccitt3 | `3` | Spécifie le schéma de compression CCITT3. |
| Ccitt4 | `4` | Spécifie le schéma de compression CCITT4. |
| Lzw | `5` | Spécifie le schéma de compression LZW. |

## Exemples

Montre comment rendre au format TIFF en utilisant le mode de compression RLE.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var options = new ImageSaveOptions(SaveFileFormat.Tiff);

// Enregistrez le projet avec la compression Rle
options.TiffCompression = TiffCompression.Rle;
project.Save(OutDir + "RenderMultipageTIFF_comp_rle_out.tif", options);
```

### Voir aussi

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


