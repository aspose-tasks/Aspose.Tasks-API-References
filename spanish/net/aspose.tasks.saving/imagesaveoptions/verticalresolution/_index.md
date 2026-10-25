---
title: "ImageSaveOptions.VerticalResolution"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad ImageSaveOptions. Obtiene o establece la resolución vertical en dpi."
type: docs
weight: 100
url: /es/net/aspose.tasks.saving/imagesaveoptions/verticalresolution/
---
## ImageSaveOptions.VerticalResolution property

Obtiene o establece la resolución vertical en dpi.

```csharp
public float VerticalResolution { get; set; }
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


