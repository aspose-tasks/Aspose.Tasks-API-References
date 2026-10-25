---
title: "PdfSaveOptions.Compliance"
second_title: "Aspose.Tasks for .NET API 참조"
description: "PdfSaveOptions 속성. 생성된 PDF 문서에 대한 원하는 준수 수준을 가져오거나 설정합니다. 기본값은 Pdf15입니다."
type: docs
weight: 20
url: /ko/net/aspose.tasks.saving/pdfsaveoptions/compliance/
---
## PdfSaveOptions.Compliance property

생성된 PDF 문서의 원하는 호환성 수준을 가져오거나 설정합니다. 기본값은 Pdf15입니다.

```csharp
public PdfCompliance Compliance { get; set; }
```

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

* enum [PdfCompliance](../../pdfcompliance/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../pdfsaveoptions/)
* assembly [Aspose.Tasks](../../../)


