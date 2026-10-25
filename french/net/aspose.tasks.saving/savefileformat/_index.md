---
title: "Énumération SaveFileFormat"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Énumération Aspose.Tasks.Saving.SaveFileFormat. Énumération pour la sélection du format d'enregistrement du projet"
type: docs
weight: 2180
url: /fr/net/aspose.tasks.saving/savefileformat/
---
## SaveFileFormat enumeration

Énumération pour la sélection du format d'enregistrement du projet.

```csharp
public enum SaveFileFormat
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Mpp | `0` | Format MPP. |
| Xml | `1` | Format XML. |
| Html | `2` | Format HTML. |
| Bmp | `3` | Format BMP. |
| Png | `4` | Format PNG. |
| Jpeg | `5` | Format JPEG. |
| Pdf | `6` | Format PDF. |
| Tiff | `7` | Format TIFF. |
| Xps | `8` | Format XPS. |
| Xaml | `9` | Format XAML. |
| Svg | `10` | Format SVG. |
| Csv | `11` | Format CSV. |
| Txt | `12` | Format texte (délimité par des tabulations). |
| Spreadsheet2003 | `13` | XML de feuille de calcul (Excel 2003). |
| Xlsx | `14` | OOXML (Office Open XML, Excel 2007+). |
| PrimaveraP6Xml | `15` | Format XML Primavera P6. |
| PrimaveraXer | `16` | Format XER Primavera PM. |
| Mpx | `17` | Format MPX. |
| GdHtml | `18` | Format HTML pour enregistrer les données du projet dans un ensemble de tables HTML. |

## Exemples

Montre comment enregistrer un projet au format CSV.

```csharp
var project = new Project(DataDir + "CreateProject1.mpp");
project.Save(OutDir + "SaveProjectAsCSV_out.csv", SaveFileFormat.Csv);
```

### Voir aussi

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


