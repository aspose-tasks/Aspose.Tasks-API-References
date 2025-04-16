---
title: Enum SaveFileFormat
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.Saving.SaveFileFormat enum. Enumeration for saving project format selection
type: docs
weight: 2120
url: /net/aspose.tasks.saving/savefileformat/
---
## SaveFileFormat enumeration

Enumeration for saving project format selection.

```csharp
public enum SaveFileFormat
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Mpp | `0` | MPP format. |
| Xml | `1` | XML format. |
| Html | `2` | HTML format. |
| Bmp | `3` | BMP format. |
| Png | `4` | PNG format. |
| Jpeg | `5` | JPEG format. |
| Pdf | `6` | PDF format. |
| Tiff | `7` | TIFF format. |
| Xps | `8` | XPS format. |
| Xaml | `9` | XAML format. |
| Svg | `10` | SVG format. |
| Csv | `11` | CSV format. |
| Txt | `12` | Text format (tab delimited). |
| Spreadsheet2003 | `13` | Spreadsheet XML (Excel 2003). |
| Xlsx | `14` | OOXML (Office Open XML, Excel 2007+). |
| PrimaveraP6Xml | `15` | Primavera P6 Xml format. |
| PrimaveraXer | `16` | Primavera PM XER format. |
| Mpx | `17` | MPX format. |
| GdHtml | `18` | Html format for saving project data in a set of html tables. |

## Examples

Shows how to save a project in CSV format.

```csharp
var project = new Project(DataDir + "CreateProject1.mpp");
project.Save(OutDir + "SaveProjectAsCSV_out.csv", SaveFileFormat.Csv);
```

### See Also

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


