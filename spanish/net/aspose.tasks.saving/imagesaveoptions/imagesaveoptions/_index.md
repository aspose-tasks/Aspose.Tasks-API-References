---
title: "ImageSaveOptions.ImageSaveOptions"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Constructor ImageSaveOptions. Inicializa una nueva instancia de la clase ImageSaveOptions que puede usarse para guardar imágenes renderizadas en formatos TIFF, PNG, BMP o JPEG."
type: docs
weight: 10
url: /es/net/aspose.tasks.saving/imagesaveoptions/imagesaveoptions/
---
## ImageSaveOptions constructor

Inicializa una nueva instancia de la clase [`ImageSaveOptions`](../) que puede usarse para guardar imágenes renderizadas en formatos TIFF, PNG, BMP o JPEG.

```csharp
public ImageSaveOptions(SaveFileFormat saveFormat)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| saveFormat | SaveFileFormat | Puede ser TIFF, PNG, BMP o JPEG[`SaveFileFormat`](../../savefileformat/). |

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentException | Se lanza si *saveFormat* no es un formato de imagen válido. Los valores válidos son TIFF, PNG, BMP o JPEG. |

## Ejemplos

Muestra cómo guardar el proyecto en un flujo como una imagen.

```csharp
var project = new Project();

using (var stream = new FileStream(OutDir + "EmptyProjectSaveStream_out.xml", FileMode.Create, FileAccess.Write))
{
    var options = new ImageSaveOptions(SaveFileFormat.Png);

    // usando ImageSaveOptions guardamos el proyecto en formato de imagen
    project.Save(stream, options);
}
```

### Ver también

* enum [SaveFileFormat](../../savefileformat/)
* class [ImageSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../imagesaveoptions/)
* assembly [Aspose.Tasks](../../../)


