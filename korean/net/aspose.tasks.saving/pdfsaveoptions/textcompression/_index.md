---
title: "PdfSaveOptions.TextCompression"
second_title: "Aspose.Tasks for .NET API 참조"
description: "PdfSaveOptions 속성. 이미지 제외 모든 콘텐츠 스트림에 사용할 압축 유형을 가져오거나 설정합니다. 기본값은 Flate입니다."
type: docs
weight: 100
url: /ko/net/aspose.tasks.saving/pdfsaveoptions/textcompression/
---
## PdfSaveOptions.TextCompression property

이미지를 제외한 모든 콘텐츠 스트림에 사용할 압축 유형을 가져오거나 설정합니다. 기본값은 Flate입니다.

```csharp
public PdfTextCompression TextCompression { get; set; }
```

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

* enum [PdfTextCompression](../../pdftextcompression/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../pdfsaveoptions/)
* assembly [Aspose.Tasks](../../../)


