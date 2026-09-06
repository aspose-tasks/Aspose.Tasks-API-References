---
title: "PdfSaveOptions.EncryptionDetails"
second_title: "Aspose.Tasks for .NET API 参考"
description: "PdfSaveOptions 属性。获取或设置加密详细信息。如果未设置，则不会执行加密。"
type: docs
weight: 40
url: /zh/net/aspose.tasks.saving/pdfsaveoptions/encryptiondetails/
---
## PdfSaveOptions.EncryptionDetails property

获取或设置加密详细信息。如果未设置，则不会执行加密。

```csharp
public PdfEncryptionDetails EncryptionDetails { get; set; }
```

## 示例

展示如何设置 PDF 文档的加密详细信息。如果未设置，则不会执行加密。

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var encryptionDetails = new PdfEncryptionDetails("userPassword", "ownerPassword", PdfEncryptionAlgorithm.RC4_128);

var options = new PdfSaveOptions();

// 设置 PDF 文档的加密详细信息
options.EncryptionDetails = encryptionDetails;

// 调整其他属性
// 设置文档将被保存的 <see cref="P:Aspose.Tasks.Saving.SaveOptions.PresentationFormat" />。
options.PresentationFormat = PresentationFormat.GanttChart;

project.Save(OutDir + "WorkWithEncryptionDetails_out.pdf", options);
```

### 另见

* class [PdfEncryptionDetails](../../pdfencryptiondetails/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../pdfsaveoptions/)
* assembly [Aspose.Tasks](../../../)


