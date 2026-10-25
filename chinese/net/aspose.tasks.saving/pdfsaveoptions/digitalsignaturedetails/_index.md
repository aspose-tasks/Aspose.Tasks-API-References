---
title: "PdfSaveOptions.DigitalSignatureDetails"
second_title: "Aspose.Tasks for .NET API 参考"
description: "PdfSaveOptions 属性。获取或设置数字签名详细信息。如果未设置，则不会执行签名。"
type: docs
weight: 30
url: /zh/net/aspose.tasks.saving/pdfsaveoptions/digitalsignaturedetails/
---
## PdfSaveOptions.DigitalSignatureDetails property

获取或设置数字签名详细信息。如果未设置，则不会执行签名。

```csharp
public PdfDigitalSignatureDetails DigitalSignatureDetails { get; set; }
```

## 示例

展示如何设置数字签名详细信息。如果未设置，则不会执行签名。

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions();
var certificate = new X509Certificate2();

// 设置数字签名详细信息。如果未设置，则不会执行签名。
options.DigitalSignatureDetails = new PdfDigitalSignatureDetails(
    certificate,
    "reason",
    "location",
    new DateTime(2019, 1, 1),
    PdfDigitalSignatureHashAlgorithm.Sha1);

// 调整其他属性
// 设置文档将被保存的 <see cref="P:Aspose.Tasks.Saving.SaveOptions.PresentationFormat" />。
options.PresentationFormat = PresentationFormat.GanttChart;

// 设置生成的 PDF 文档的期望符合级别
options.Compliance = PdfCompliance.PdfA1b;

project.Save(OutDir + "WorkWithDigitalSignatureDetails_out.pdf", options);
```

### 另见

* class [PdfDigitalSignatureDetails](../../pdfdigitalsignaturedetails/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../pdfsaveoptions/)
* assembly [Aspose.Tasks](../../../)


