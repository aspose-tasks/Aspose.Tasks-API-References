---
title: "열거형 PdfTextCompression"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.Saving.PdfTextCompression 열거형. 이미지 제외 모든 PDF 파일 내용에 적용되는 압축 유형을 지정합니다."
type: docs
weight: 2140
url: /ko/net/aspose.tasks.saving/pdftextcompression/
---
## PdfTextCompression enumeration

이미지를 제외한 PDF 파일의 모든 콘텐츠에 적용되는 압축 유형을 지정합니다.

```csharp
public enum PdfTextCompression
```

### 값들

| 이름 | 값 | 설명 |
| --- | --- | --- |
| None | `0` | 압축 없음. |
| Flate | `1` | Flate 압축. |

## 예제

이미지를 제외한 모든 콘텐츠 스트림에 사용할 압축 유형을 설정하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions();

// 이미지를 제외한 모든 콘텐츠 스트림에 사용할 압축 유형을 설정합니다
options.TextCompression = PdfTextCompression.Flate;

// 추가 속성을 조정합니다
// 문서가 저장될 <see cref=\"P:Aspose.Tasks.Saving.SaveOptions.PresentationFormat\" />를 설정합니다.
options.PresentationFormat = PresentationFormat.GanttChart;

// 생성된 PDF 문서에 원하는 적합성 수준을 설정합니다
options.Compliance = PdfCompliance.PdfA1b;

project.Save(OutDir + "WorkWithTextCompression_out.pdf", options);
```

### 또 보기

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


