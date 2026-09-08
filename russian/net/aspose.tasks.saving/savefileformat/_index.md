---
title: "Перечисление SaveFileFormat"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Перечисление Aspose.Tasks.Saving.SaveFileFormat. Перечисление для выбора формата сохранения проекта."
type: docs
weight: 2180
url: /ru/net/aspose.tasks.saving/savefileformat/
---
## SaveFileFormat enumeration

Перечисление для выбора формата сохранения проекта.

```csharp
public enum SaveFileFormat
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Mpp | `0` | Формат MPP. |
| Xml | `1` | Формат XML. |
| Html | `2` | Формат HTML. |
| Bmp | `3` | Формат BMP. |
| Png | `4` | Формат PNG. |
| Jpeg | `5` | Формат JPEG. |
| Pdf | `6` | Формат PDF. |
| Tiff | `7` | Формат TIFF. |
| Xps | `8` | Формат XPS. |
| Xaml | `9` | Формат XAML. |
| Svg | `10` | Формат SVG. |
| Csv | `11` | Формат CSV. |
| Txt | `12` | Текстовый формат (разделённый табуляцией). |
| Spreadsheet2003 | `13` | Spreadsheet XML (Excel 2003). |
| Xlsx | `14` | OOXML (Office Open XML, Excel 2007+). |
| PrimaveraP6Xml | `15` | Primavera P6 Xml формат. |
| PrimaveraXer | `16` | Primavera PM XER формат. |
| Mpx | `17` | Формат MPX. |
| GdHtml | `18` | HTML-формат для сохранения данных проекта в наборе HTML-таблиц. |

## Примеры

Показывает, как сохранить проект в формате CSV.

```csharp
var project = new Project(DataDir + "CreateProject1.mpp");
project.Save(OutDir + "SaveProjectAsCSV_out.csv", SaveFileFormat.Csv);
```

### См. также

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


