---
title: "PdfSaveOptions.TextCompression"
second_title: "Aspose.Tasks for .NET API 参考"
description: "PdfSaveOptions 属性。获取或设置用于除图像外所有内容流的压缩类型。默认是 Flate"
type: docs
weight: 100
url: /zh/net/aspose.tasks.saving/pdfsaveoptions/textcompression/
---
## PdfSaveOptions.TextCompression property

获取或设置除图像外所有内容流使用的压缩类型。默认是 Flate。

```csharp
public PdfTextCompression TextCompression { get; set; }
```

## 示例

展示如何设置一种压缩类型，以用于除图像之外的所有内容流。

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions();

// 设置用于除图像之外的所有内容流的压缩类型
options.TextCompression = PdfTextCompression.Flate;

// 调整其他属性
// 设置文档将被保存的 <see cref="P:Aspose.Tasks.Saving.SaveOptions.PresentationFormat" />。
options.PresentationFormat = PresentationFormat.GanttChart;

// 设置生成的 PDF 文档的期望符合级别
options.Compliance = PdfCompliance.PdfA1b;

project.Save(OutDir + "WorkWithTextCompression_out.pdf", options);
```

### 另见

* enum [PdfTextCompression](../../pdftextcompression/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../pdfsaveoptions/)
* assembly [Aspose.Tasks](../../../)


