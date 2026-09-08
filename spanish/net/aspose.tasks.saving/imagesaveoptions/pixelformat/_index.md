---
title: "ImageSaveOptions.PixelFormat"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad ImageSaveOptions. Obtiene o establece el formato de los datos de color para cada píxel en la imagen."
type: docs
weight: 70
url: /es/net/aspose.tasks.saving/imagesaveoptions/pixelformat/
---
## ImageSaveOptions.PixelFormat property

Obtiene o establece el formato de los datos de color para cada píxel en la imagen.

```csharp
public PixelFormat PixelFormat { get; set; }
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


