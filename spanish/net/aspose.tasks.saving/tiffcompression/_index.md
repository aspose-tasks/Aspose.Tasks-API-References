---
title: "Enumeración TiffCompression"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Enumeración Aspose.Tasks.Saving.TiffCompression. Especifica qué tipo de compresión aplicar al guardar páginas en el formato TIFF"
type: docs
weight: 2250
url: /es/net/aspose.tasks.saving/tiffcompression/
---
## TiffCompression enumeration

Especifica qué tipo de compresión aplicar al guardar páginas en formato TIFF.

```csharp
public enum TiffCompression
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| None | `1` | Especifica sin compresión. |
| Rle | `2` | Especifica el esquema de compresión RLE. |
| Ccitt3 | `3` | Especifica el esquema de compresión CCITT3. |
| Ccitt4 | `4` | Especifica el esquema de compresión CCITT4. |
| Lzw | `5` | Especifica el esquema de compresión LZW. |

## Ejemplos

Muestra cómo renderizar en formato TIFF usando el modo de compresión RLE.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var options = new ImageSaveOptions(SaveFileFormat.Tiff);

// Guardar el proyecto con compresión Rle
options.TiffCompression = TiffCompression.Rle;
project.Save(OutDir + "RenderMultipageTIFF_comp_rle_out.tif", options);
```

### Ver también

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


