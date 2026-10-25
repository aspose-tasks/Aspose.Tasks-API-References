---
title: "열거형 SaveFileFormat"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.Saving.SaveFileFormat 열거형. 프로젝트 저장 형식 선택을 위한 열거형입니다."
type: docs
weight: 2180
url: /ko/net/aspose.tasks.saving/savefileformat/
---
## SaveFileFormat enumeration

프로젝트 형식 선택 저장을 위한 열거형입니다.

```csharp
public enum SaveFileFormat
```

### 값들

| 이름 | 값 | 설명 |
| --- | --- | --- |
| Mpp | `0` | MPP 형식. |
| Xml | `1` | XML 형식. |
| Html | `2` | HTML 형식. |
| Bmp | `3` | BMP 형식. |
| Png | `4` | PNG 형식. |
| Jpeg | `5` | JPEG 형식. |
| Pdf | `6` | PDF 형식. |
| Tiff | `7` | TIFF 형식. |
| Xps | `8` | XPS 형식. |
| Xaml | `9` | XAML 형식. |
| Svg | `10` | SVG 형식. |
| Csv | `11` | CSV 형식. |
| Txt | `12` | 텍스트 형식(탭 구분). |
| Spreadsheet2003 | `13` | 스프레드시트 XML(Excel 2003). |
| Xlsx | `14` | OOXML(Office Open XML, Excel 2007+). |
| PrimaveraP6Xml | `15` | Primavera P6 Xml 형식. |
| PrimaveraXer | `16` | Primavera PM XER 형식. |
| Mpx | `17` | MPX 형식. |
| GdHtml | `18` | Html 형식은 프로젝트 데이터를 일련의 html 테이블에 저장합니다. |

## 예제

CSV 형식으로 프로젝트를 저장하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "CreateProject1.mpp");
project.Save(OutDir + "SaveProjectAsCSV_out.csv", SaveFileFormat.Csv);
```

### 또 보기

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


