---
title: "Απαρίθμηση SaveFileFormat"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Απαρίθμηση Aspose.Tasks.Saving.SaveFileFormat. Καταγραφή για την επιλογή μορφής αποθήκευσης του έργου"
type: docs
weight: 2180
url: /el/net/aspose.tasks.saving/savefileformat/
---
## SaveFileFormat enumeration

Απαρίθμηση για την επιλογή μορφής αποθήκευσης έργου.

```csharp
public enum SaveFileFormat
```

### Τιμές

| Όνομα | Τιμή | Περιγραφή |
| --- | --- | --- |
| Mpp | `0` | Μορφή MPP. |
| Xml | `1` | Μορφή XML. |
| Html | `2` | Μορφή HTML. |
| Bmp | `3` | Μορφή BMP. |
| Png | `4` | Μορφή PNG. |
| Jpeg | `5` | Μορφή JPEG. |
| Pdf | `6` | Μορφή PDF. |
| Tiff | `7` | Μορφή TIFF. |
| Xps | `8` | Μορφή XPS. |
| Xaml | `9` | μορφή XAML. |
| Svg | `10` | μορφή SVG. |
| Csv | `11` | μορφή CSV. |
| Txt | `12` | Μορφή κειμένου (με διαχωριστικό καρτέλας). |
| Spreadsheet2003 | `13` | Spreadsheet XML (Excel 2003). |
| Xlsx | `14` | OOXML (Office Open XML, Excel 2007+). |
| PrimaveraP6Xml | `15` | Primavera P6 Xml format. |
| PrimaveraXer | `16` | Primavera PM XER format. |
| Mpx | `17` | MPX format. |
| GdHtml | `18` | Μορφή Html για αποθήκευση δεδομένων έργου σε ένα σύνολο πινάκων html. |

## Παραδείγματα

Δείχνει πώς να αποθηκεύσετε ένα έργο σε μορφή CSV.

```csharp
var project = new Project(DataDir + "CreateProject1.mpp");
project.Save(OutDir + "SaveProjectAsCSV_out.csv", SaveFileFormat.Csv);
```

### Δείτε επίσης

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


