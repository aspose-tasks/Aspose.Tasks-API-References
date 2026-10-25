---
title: "Enum SaveFileFormat"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.Saving.SaveFileFormat enum. Proje formatı seçimi için kaydetme enumerasyonu"
type: docs
weight: 2180
url: /tr/net/aspose.tasks.saving/savefileformat/
---
## SaveFileFormat enumeration

Proje formatı seçiminin kaydedilmesi için enum.

```csharp
public enum SaveFileFormat
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Mpp | `0` | MPP formatı. |
| Xml | `1` | XML formatı. |
| Html | `2` | HTML formatı. |
| Bmp | `3` | BMP formatı. |
| Png | `4` | PNG formatı. |
| Jpeg | `5` | JPEG formatı. |
| Pdf | `6` | PDF formatı. |
| Tiff | `7` | TIFF formatı. |
| Xps | `8` | XPS formatı. |
| Xaml | `9` | XAML formatı. |
| Svg | `10` | SVG formatı. |
| Csv | `11` | CSV formatı. |
| Txt | `12` | Metin formatı (sekme ile ayrılmış). |
| Spreadsheet2003 | `13` | Elektronik tablo XML (Excel 2003). |
| Xlsx | `14` | OOXML (Office Open XML, Excel 2007+). |
| PrimaveraP6Xml | `15` | Primavera P6 Xml formatı. |
| PrimaveraXer | `16` | Primavera PM XER formatı. |
| Mpx | `17` | MPX formatı. |
| GdHtml | `18` | Proje verilerini bir dizi HTML tablosunda kaydetmek için HTML formatı. |

## Örnekler

Bir projeyi CSV formatında nasıl kaydedeceğinizi gösterir.

```csharp
var project = new Project(DataDir + "CreateProject1.mpp");
project.Save(OutDir + "SaveProjectAsCSV_out.csv", SaveFileFormat.Csv);
```

### Ayrıca Bakınız

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


