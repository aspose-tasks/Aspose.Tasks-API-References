---
title: "Enumeración SaveFileFormat"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Enumeración Aspose.Tasks.Saving.SaveFileFormat. Enumeración para la selección del formato de guardado del proyecto"
type: docs
weight: 2180
url: /es/net/aspose.tasks.saving/savefileformat/
---
## SaveFileFormat enumeration

Enumeración para la selección del formato de guardado del proyecto.

```csharp
public enum SaveFileFormat
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Mpp | `0` | Formato MPP. |
| Xml | `1` | Formato XML. |
| Html | `2` | Formato HTML. |
| Bmp | `3` | Formato BMP. |
| Png | `4` | Formato PNG. |
| Jpeg | `5` | Formato JPEG. |
| Pdf | `6` | Formato PDF. |
| Tiff | `7` | Formato TIFF. |
| Xps | `8` | Formato XPS. |
| Xaml | `9` | Formato XAML. |
| Svg | `10` | Formato SVG. |
| Csv | `11` | Formato CSV. |
| Txt | `12` | Formato de texto (delimitado por tabulaciones). |
| Spreadsheet2003 | `13` | XML de hoja de cálculo (Excel 2003). |
| Xlsx | `14` | OOXML (Office Open XML, Excel 2007+). |
| PrimaveraP6Xml | `15` | Formato XML de Primavera P6. |
| PrimaveraXer | `16` | Formato XER de Primavera PM. |
| Mpx | `17` | Formato MPX. |
| GdHtml | `18` | Formato HTML para guardar datos del proyecto en un conjunto de tablas HTML. |

## Ejemplos

Muestra cómo guardar un proyecto en formato CSV.

```csharp
var project = new Project(DataDir + "CreateProject1.mpp");
project.Save(OutDir + "SaveProjectAsCSV_out.csv", SaveFileFormat.Csv);
```

### Ver también

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


