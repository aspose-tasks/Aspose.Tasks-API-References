---
title: "PdfSaveOptions.Compliance"
second_title: "Aspose.Tasks for .NET API 参考"
description: "PdfSaveOptions 属性。获取或设置生成的 PDF 文档的期望合规级别。默认是 Pdf15。"
type: docs
weight: 20
url: /zh/net/aspose.tasks.saving/pdfsaveoptions/compliance/
---
## PdfSaveOptions.Compliance property

获取或设置生成的 PDF 文档的期望合规级别。默认是 Pdf15。

```csharp
public PdfCompliance Compliance { get; set; }
```

## 示例

展示如何为生成的 PDF 文档设置所需的合规级别。

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions();

// 设置生成的 PDF 文档的期望符合级别
// 默认是 <see cref="PdfCompliance.Pdf15"/> 类型
options.Compliance = PdfCompliance.PdfA1b;

// 调整其他属性
// 设置文档将被保存的 <see cref="P:Aspose.Tasks.Saving.SaveOptions.PresentationFormat" />。
options.PresentationFormat = PresentationFormat.GanttChart;

project.Save(OutDir + "WorkWithPdfCompliance_out.pdf", options);
```

### 另见

* enum [PdfCompliance](../../pdfcompliance/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../pdfsaveoptions/)
* assembly [Aspose.Tasks](../../../)


