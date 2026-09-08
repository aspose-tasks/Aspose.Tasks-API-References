---
title: "PdfSaveOptions.EncryptionDetails"
second_title: "Aspose.Tasks for .NET API 참조"
description: "PdfSaveOptions 속성. 암호화 세부 정보를 가져오거나 설정합니다. 설정되지 않으면 암호화가 수행되지 않습니다."
type: docs
weight: 40
url: /ko/net/aspose.tasks.saving/pdfsaveoptions/encryptiondetails/
---
## PdfSaveOptions.EncryptionDetails property

암호화 세부 정보를 가져오거나 설정합니다. 설정하지 않으면 암호화가 수행되지 않습니다.

```csharp
public PdfEncryptionDetails EncryptionDetails { get; set; }
```

## 예제

PDF 문서의 암호화 세부 정보를 설정하는 방법을 보여줍니다. 설정되지 않으면 암호화가 수행되지 않습니다.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var encryptionDetails = new PdfEncryptionDetails("userPassword", "ownerPassword", PdfEncryptionAlgorithm.RC4_128);

var options = new PdfSaveOptions();

// PDF 문서의 암호화 세부 정보를 설정합니다.
options.EncryptionDetails = encryptionDetails;

// 추가 속성을 조정합니다
// 문서가 저장될 <see cref=\"P:Aspose.Tasks.Saving.SaveOptions.PresentationFormat\" />를 설정합니다.
options.PresentationFormat = PresentationFormat.GanttChart;

project.Save(OutDir + "WorkWithEncryptionDetails_out.pdf", options);
```

### 또 보기

* class [PdfEncryptionDetails](../../pdfencryptiondetails/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../pdfsaveoptions/)
* assembly [Aspose.Tasks](../../../)


