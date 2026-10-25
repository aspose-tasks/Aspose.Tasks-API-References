---
title: "열거형 PdfCompliance"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.Saving.PdfCompliance 열거형. 출력 파일의 PDF 준수 수준을 지정합니다."
type: docs
weight: 2070
url: /ko/net/aspose.tasks.saving/pdfcompliance/
---
## PdfCompliance enumeration

출력 파일의 PDF 준수 수준을 지정합니다.

```csharp
public enum PdfCompliance
```

### 값들

| 이름 | 값 | 설명 |
| --- | --- | --- |
| Pdf15 | `0` | PDF/15 준수 수준. |
| PdfA1a | `1` | PDF/A-1a 준수 수준. |
| PdfA1b | `2` | PDF/A-1b 준수 수준. |

## 예제

생성된 PDF 문서에 원하는 준수 수준을 설정하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions();

// 생성된 PDF 문서에 원하는 적합성 수준을 설정합니다
// 기본값은 <see cref=\"PdfCompliance.Pdf15\"/> 유형입니다.
options.Compliance = PdfCompliance.PdfA1b;

// 추가 속성을 조정합니다
// 문서가 저장될 <see cref=\"P:Aspose.Tasks.Saving.SaveOptions.PresentationFormat\" />를 설정합니다.
options.PresentationFormat = PresentationFormat.GanttChart;

project.Save(OutDir + "WorkWithPdfCompliance_out.pdf", options);
```

### 또 보기

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


