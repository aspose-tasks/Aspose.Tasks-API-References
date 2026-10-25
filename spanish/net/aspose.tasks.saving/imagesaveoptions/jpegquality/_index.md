---
title: "ImageSaveOptions.JpegQuality"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad ImageSaveOptions. Obtiene o establece la calidad JPEG. El rango de valores permitido es 0..100"
type: docs
weight: 40
url: /es/net/aspose.tasks.saving/imagesaveoptions/jpegquality/
---
## ImageSaveOptions.JpegQuality property

Obtiene o establece la calidad JPEG. El rango de valores permitido es 0..100.

```csharp
public int JpegQuality { get; set; }
```

## Ejemplos

Muestra cómo establecer la calidad JPEG de los archivos JPEG de salida.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

// Para manipular la calidad JPEG se puede usar la propiedad ImageSaveOptions.JpegQuality.
// El rango de valores permitido es 0..100.
var options = new ImageSaveOptions(SaveFileFormat.Jpeg)
{
    JpegQuality = 50
};

project.Save(OutDir + "SaveProjectAsJPEG_out.jpeg", options);
```

### Ver también

* class [ImageSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../imagesaveoptions/)
* assembly [Aspose.Tasks](../../../)


