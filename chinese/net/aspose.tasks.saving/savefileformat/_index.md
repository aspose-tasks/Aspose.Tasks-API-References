---
title: "枚举 SaveFileFormat"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.Saving.SaveFileFormat 枚举。用于选择保存项目格式的枚举"
type: docs
weight: 2180
url: /zh/net/aspose.tasks.saving/savefileformat/
---
## SaveFileFormat enumeration

用于保存项目格式选择的枚举。

```csharp
public enum SaveFileFormat
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| Mpp | `0` | MPP 格式。 |
| Xml | `1` | XML 格式。 |
| Html | `2` | HTML 格式。 |
| Bmp | `3` | BMP 格式。 |
| Png | `4` | PNG 格式。 |
| Jpeg | `5` | JPEG 格式。 |
| Pdf | `6` | PDF 格式。 |
| Tiff | `7` | TIFF 格式。 |
| Xps | `8` | XPS 格式。 |
| Xaml | `9` | XAML 格式。 |
| Svg | `10` | SVG 格式。 |
| Csv | `11` | CSV 格式。 |
| Txt | `12` | 文本格式（制表符分隔）。 |
| Spreadsheet2003 | `13` | 电子表格 XML（Excel 2003）。 |
| Xlsx | `14` | OOXML（Office Open XML，Excel 2007 及以上）。 |
| PrimaveraP6Xml | `15` | Primavera P6 Xml 格式。 |
| PrimaveraXer | `16` | Primavera PM XER 格式。 |
| Mpx | `17` | MPX 格式。 |
| GdHtml | `18` | Html 格式，用于将项目数据保存为一组 html 表格。 |

## 示例

展示如何以 CSV 格式保存项目。

```csharp
var project = new Project(DataDir + "CreateProject1.mpp");
project.Save(OutDir + "SaveProjectAsCSV_out.csv", SaveFileFormat.Csv);
```

### 另见

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


