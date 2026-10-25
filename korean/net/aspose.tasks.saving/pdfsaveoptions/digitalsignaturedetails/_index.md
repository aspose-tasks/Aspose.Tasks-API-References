---
title: "PdfSaveOptions.DigitalSignatureDetails"
second_title: "Aspose.Tasks for .NET API 참조"
description: "PdfSaveOptions 속성. 디지털 서명 세부 정보를 가져오거나 설정합니다. 설정되지 않으면 서명이 수행되지 않습니다."
type: docs
weight: 30
url: /ko/net/aspose.tasks.saving/pdfsaveoptions/digitalsignaturedetails/
---
## PdfSaveOptions.DigitalSignatureDetails property

디지털 서명 세부 정보를 가져오거나 설정합니다. 설정하지 않으면 서명이 수행되지 않습니다.

```csharp
public PdfDigitalSignatureDetails DigitalSignatureDetails { get; set; }
```

## 예제

디지털 서명 세부 정보를 설정하는 방법을 보여줍니다. 설정되지 않으면 서명이 수행되지 않습니다.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions();
var certificate = new X509Certificate2();

// 디지털 서명 세부 정보를 설정합니다. 설정되지 않으면 서명이 수행되지 않습니다.
options.DigitalSignatureDetails = new PdfDigitalSignatureDetails(
    certificate,
    "reason",
    "location",
    new DateTime(2019, 1, 1),
    PdfDigitalSignatureHashAlgorithm.Sha1);

// 추가 속성을 조정합니다
// 문서가 저장될 <see cref=\"P:Aspose.Tasks.Saving.SaveOptions.PresentationFormat\" />를 설정합니다.
options.PresentationFormat = PresentationFormat.GanttChart;

// 생성된 PDF 문서에 원하는 적합성 수준을 설정합니다
options.Compliance = PdfCompliance.PdfA1b;

project.Save(OutDir + "WorkWithDigitalSignatureDetails_out.pdf", options);
```

### 또 보기

* class [PdfDigitalSignatureDetails](../../pdfdigitalsignaturedetails/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../pdfsaveoptions/)
* assembly [Aspose.Tasks](../../../)


