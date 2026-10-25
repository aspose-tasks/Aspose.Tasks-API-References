---
title: "枚举 PdfTextCompression"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.Saving.PdfTextCompression 枚举。指定除图像外应用于 PDF 文件中所有内容的压缩类型。"
type: docs
weight: 2140
url: /zh/net/aspose.tasks.saving/pdftextcompression/
---
## PdfTextCompression enumeration

指定除图像外对 PDF 文件所有内容应用的压缩类型。

```csharp
public enum PdfTextCompression
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| None | `0` | 无压缩。 |
| Flate | `1` | Flate 压缩。 |

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

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


