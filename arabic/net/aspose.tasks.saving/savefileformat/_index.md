---
title: "التعداد SaveFileFormat"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "التعداد Aspose.Tasks.Saving.SaveFileFormat. تعداد لاختيار تنسيق حفظ المشروع."
type: docs
weight: 2180
url: /ar/net/aspose.tasks.saving/savefileformat/
---
## SaveFileFormat enumeration

تعداد لاختيار تنسيق حفظ المشروع.

```csharp
public enum SaveFileFormat
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Mpp | `0` | تنسيق MPP. |
| Xml | `1` | تنسيق XML. |
| Html | `2` | تنسيق HTML. |
| Bmp | `3` | تنسيق BMP. |
| Png | `4` | تنسيق PNG. |
| Jpeg | `5` | تنسيق JPEG. |
| Pdf | `6` | تنسيق PDF. |
| Tiff | `7` | تنسيق TIFF. |
| Xps | `8` | تنسيق XPS. |
| Xaml | `9` | تنسيق XAML. |
| Svg | `10` | تنسيق SVG. |
| Csv | `11` | تنسيق CSV. |
| Txt | `12` | تنسيق نص (مفصول بعلامات جدولة). |
| Spreadsheet2003 | `13` | XML للجدول (Excel 2003). |
| Xlsx | `14` | OOXML (Office Open XML، Excel 2007+). |
| PrimaveraP6Xml | `15` | تنسيق Primavera P6 Xml. |
| PrimaveraXer | `16` | تنسيق Primavera PM XER. |
| Mpx | `17` | تنسيق MPX. |
| GdHtml | `18` | تنسيق Html لحفظ بيانات المشروع في مجموعة من جداول html. |

## الأمثلة

يوضح كيفية حفظ مشروع بتنسيق CSV.

```csharp
var project = new Project(DataDir + "CreateProject1.mpp");
project.Save(OutDir + "SaveProjectAsCSV_out.csv", SaveFileFormat.Csv);
```

### انظر أيضًا

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


