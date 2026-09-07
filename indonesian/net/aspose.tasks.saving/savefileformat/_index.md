---
title: "Enum SaveFileFormat"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Enum Aspose.Tasks.Saving.SaveFileFormat. Enumerasi untuk pemilihan format penyimpanan proyek"
type: docs
weight: 2180
url: /id/net/aspose.tasks.saving/savefileformat/
---
## SaveFileFormat enumeration

Enumerasi untuk pemilihan format penyimpanan proyek.

```csharp
public enum SaveFileFormat
```

### Nilai

| Nama | Nilai | Deskripsi |
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
| Xaml | `9` | format XAML. |
| Svg | `10` | format SVG. |
| Csv | `11` | format CSV. |
| Txt | `12` | Format teks (dipisahkan tab). |
| Spreadsheet2003 | `13` | Spreadsheet XML (Excel 2003). |
| Xlsx | `14` | OOXML (Office Open XML, Excel 2007+). |
| PrimaveraP6Xml | `15` | format Primavera P6 Xml. |
| PrimaveraXer | `16` | format Primavera PM XER. |
| Mpx | `17` | format MPX. |
| GdHtml | `18` | Format Html untuk menyimpan data proyek dalam sekumpulan tabel html. |

## Contoh

Menampilkan cara menyimpan proyek dalam format CSV.

```csharp
var project = new Project(DataDir + "CreateProject1.mpp");
project.Save(OutDir + "SaveProjectAsCSV_out.csv", SaveFileFormat.Csv);
```

### Lihat Juga

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


