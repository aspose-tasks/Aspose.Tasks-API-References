---
title: "Enum SaveFileFormat"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Enum Aspose.Tasks.Saving.SaveFileFormat. Enumerazione per la selezione del formato di salvataggio del progetto"
type: docs
weight: 2180
url: /it/net/aspose.tasks.saving/savefileformat/
---
## SaveFileFormat enumeration

Enumerazione per la selezione del formato di salvataggio del progetto.

```csharp
public enum SaveFileFormat
```

### Valori

| Nome | Valore | Descrizione |
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
| Txt | `12` | Formato testo (delimitato da tabulazioni). |
| Spreadsheet2003 | `13` | XML foglio di calcolo (Excel 2003). |
| Xlsx | `14` | OOXML (Office Open XML, Excel 2007+). |
| PrimaveraP6Xml | `15` | Formato XML Primavera P6. |
| PrimaveraXer | `16` | Formato XER Primavera PM. |
| Mpx | `17` | Formato MPX. |
| GdHtml | `18` | Formato HTML per salvare i dati del progetto in un insieme di tabelle HTML. |

## Esempi

Mostra come salvare un progetto in formato CSV.

```csharp
var project = new Project(DataDir + "CreateProject1.mpp");
project.Save(OutDir + "SaveProjectAsCSV_out.csv", SaveFileFormat.Csv);
```

### Vedi anche

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


