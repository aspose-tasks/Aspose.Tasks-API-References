---
title: "ImageSaveOptions.TiffCompression"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad ImageSaveOptions. Obtiene o establece el tipo de compresión a aplicar al guardar imágenes generadas en formato TIFF"
type: docs
weight: 90
url: /es/net/aspose.tasks.saving/imagesaveoptions/tiffcompression/
---
## ImageSaveOptions.TiffCompression property

Obtiene o establece el tipo de compresión a aplicar al guardar imágenes generadas en formato TIFF.

```csharp
public TiffCompression TiffCompression { get; set; }
```

## Observaciones

Tiene efecto solo al guardar en TIFF. El valor predeterminado es `LZW`.

## Ejemplos

Muestra cómo establecer la compresión TIFF de los archivos TIFF de salida.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// Para manipular la compresión TIFF podemos usar la propiedad ImageSaveOptions.TiffCompression.
var options = new ImageSaveOptions(SaveFileFormat.Tiff)
{
    TiffCompression = TiffCompression.Lzw
};

project.Save(OutDir + "SaveProjectAsTiff_out.tif", options);
```

### Ver también

* enum [TiffCompression](../../tiffcompression/)
* class [ImageSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../imagesaveoptions/)
* assembly [Aspose.Tasks](../../../)


