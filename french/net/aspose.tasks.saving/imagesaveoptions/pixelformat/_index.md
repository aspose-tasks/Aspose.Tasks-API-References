---
title: "ImageSaveOptions.PixelFormat"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété ImageSaveOptions. Obtient ou définit le format des données de couleur pour chaque pixel de l'image"
type: docs
weight: 70
url: /fr/net/aspose.tasks.saving/imagesaveoptions/pixelformat/
---
## ImageSaveOptions.PixelFormat property

Obtient ou définit le format des données de couleur pour chaque pixel de l'image.

```csharp
public PixelFormat PixelFormat { get; set; }
```

## Exemples

Montre comment définir le format de pixel qui est utilisé lors de la conversion en formats d'image.

```csharp
var project = new Project(DataDir + "Project1.mpp");
var options = new ImageSaveOptions(SaveFileFormat.Tiff);
options.HorizontalResolution = 72;
options.VerticalResolution = 72;
options.PixelFormat = PixelFormat.Format24bppRgb;
project.Save(OutDir + "RenderProjectDataToFormat24bppRgb_out.tif", options);
```

### Voir aussi

* class [ImageSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../imagesaveoptions/)
* assembly [Aspose.Tasks](../../../)


