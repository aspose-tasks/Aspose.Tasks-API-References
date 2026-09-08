---
title: "ImageSaveOptions.HorizontalResolution"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad ImageSaveOptions. Obtiene o establece la resolución horizontal en dpi"
type: docs
weight: 30
url: /es/net/aspose.tasks.saving/imagesaveoptions/horizontalresolution/
---
## ImageSaveOptions.HorizontalResolution property

Obtiene o establece la resolución horizontal en dpi.

```csharp
public float HorizontalResolution { get; set; }
```

## Ejemplos

Muestra cómo establecer el formato de píxel que se utiliza durante la conversión a formatos de imagen.

```csharp
var project = new Project(DataDir + "Project1.mpp");
var options = new ImageSaveOptions(SaveFileFormat.Tiff);
options.HorizontalResolution = 72;
options.VerticalResolution = 72;
options.PixelFormat = PixelFormat.Format24bppRgb;
project.Save(OutDir + "RenderProjectDataToFormat24bppRgb_out.tif", options);
```

### Ver también

* class [ImageSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../imagesaveoptions/)
* assembly [Aspose.Tasks](../../../)


