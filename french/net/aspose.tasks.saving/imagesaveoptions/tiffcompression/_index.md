---
title: "ImageSaveOptions.TiffCompression"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété ImageSaveOptions. Obtient ou définit le type de compression à appliquer lors de l'enregistrement des images générées au format TIFF"
type: docs
weight: 90
url: /fr/net/aspose.tasks.saving/imagesaveoptions/tiffcompression/
---
## ImageSaveOptions.TiffCompression property

Obtient ou définit le type de compression à appliquer lors de l'enregistrement des images générées au format TIFF.

```csharp
public TiffCompression TiffCompression { get; set; }
```

## Remarques

N'a d'effet que lors de l'enregistrement au format TIFF. La valeur par défaut est `LZW`.

## Exemples

Montre comment définir la compression TIFF des fichiers TIFF de sortie.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// Afin de manipuler la compression TIFF, nous pouvons utiliser la propriété ImageSaveOptions.TiffCompression.
var options = new ImageSaveOptions(SaveFileFormat.Tiff)
{
    TiffCompression = TiffCompression.Lzw
};

project.Save(OutDir + "SaveProjectAsTiff_out.tif", options);
```

### Voir aussi

* enum [TiffCompression](../../tiffcompression/)
* class [ImageSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../imagesaveoptions/)
* assembly [Aspose.Tasks](../../../)


