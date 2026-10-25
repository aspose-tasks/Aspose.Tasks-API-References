---
title: "ImageSaveOptions.ImageSaveOptions"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Constructeur ImageSaveOptions. Initialise une nouvelle instance de la classe ImageSaveOptions qui peut être utilisée pour enregistrer des images rendues aux formats TIFF, PNG, BMP ou JPEG"
type: docs
weight: 10
url: /fr/net/aspose.tasks.saving/imagesaveoptions/imagesaveoptions/
---
## ImageSaveOptions constructor

Initialise une nouvelle instance de la classe [`ImageSaveOptions`](../) qui peut être utilisée pour enregistrer des images rendues aux formats TIFF, PNG, BMP ou JPEG.

```csharp
public ImageSaveOptions(SaveFileFormat saveFormat)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| saveFormat | SaveFileFormat | Peut être TIFF, PNG, BMP ou JPEG[`SaveFileFormat`](../../savefileformat/). |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentException | Lancé si *saveFormat* n'est pas un format d'image valide. Les valeurs valides sont TIFF, PNG, BMP ou JPEG. |

## Exemples

Montre comment enregistrer le projet dans un flux sous forme d'image.

```csharp
var project = new Project();

using (var stream = new FileStream(OutDir + "EmptyProjectSaveStream_out.xml", FileMode.Create, FileAccess.Write))
{
    var options = new ImageSaveOptions(SaveFileFormat.Png);

    // en utilisant ImageSaveOptions, nous enregistrons le projet au format image
    project.Save(stream, options);
}
```

### Voir aussi

* enum [SaveFileFormat](../../savefileformat/)
* class [ImageSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../imagesaveoptions/)
* assembly [Aspose.Tasks](../../../)


