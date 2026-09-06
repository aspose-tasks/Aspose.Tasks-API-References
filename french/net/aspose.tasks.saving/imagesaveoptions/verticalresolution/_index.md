---
title: "ImageSaveOptions.VerticalResolution"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété ImageSaveOptions. Obtient ou définit la résolution verticale en dpi"
type: docs
weight: 100
url: /fr/net/aspose.tasks.saving/imagesaveoptions/verticalresolution/
---
## ImageSaveOptions.VerticalResolution property

Obtient ou définit la résolution verticale en dpi.

```csharp
public float VerticalResolution { get; set; }
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


