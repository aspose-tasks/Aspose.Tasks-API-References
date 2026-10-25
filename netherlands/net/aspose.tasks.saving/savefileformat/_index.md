---
title: "Enum SaveFileFormat"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.Saving.SaveFileFormat‑enum. Enumeratie voor de selectie van het projectopslagformaat"
type: docs
weight: 2180
url: /nl/net/aspose.tasks.saving/savefileformat/
---
## SaveFileFormat enumeration

Enumeratie voor het opslaan van projectformaatselectie.

```csharp
public enum SaveFileFormat
```

### Waarden

| Naam | Waarde | Beschrijving |
| --- | --- | --- |
| Mpp | `0` | MPP‑formaat. |
| Xml | `1` | XML‑formaat. |
| Html | `2` | HTML‑formaat. |
| Bmp | `3` | BMP‑formaat. |
| Png | `4` | PNG‑formaat. |
| Jpeg | `5` | JPEG‑formaat. |
| Pdf | `6` | PDF‑formaat. |
| Tiff | `7` | TIFF‑formaat. |
| Xps | `8` | XPS‑formaat. |
| Xaml | `9` | XAML-indeling. |
| Svg | `10` | SVG-indeling. |
| Csv | `11` | CSV-indeling. |
| Txt | `12` | Tekstindeling (tab-gescheiden). |
| Spreadsheet2003 | `13` | Spreadsheet XML (Excel 2003). |
| Xlsx | `14` | OOXML (Office Open XML, Excel 2007+). |
| PrimaveraP6Xml | `15` | Primavera P6 XML-indeling. |
| PrimaveraXer | `16` | Primavera PM XER-indeling. |
| Mpx | `17` | MPX-indeling. |
| GdHtml | `18` | Html-indeling voor het opslaan van projectgegevens in een reeks html-tabellen. |

## Voorbeelden

Toont hoe een project op te slaan in CSV-indeling.

```csharp
var project = new Project(DataDir + "CreateProject1.mpp");
project.Save(OutDir + "SaveProjectAsCSV_out.csv", SaveFileFormat.Csv);
```

### Zie ook

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


