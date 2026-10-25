---
title: "枚举 PdfCompliance"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.Saving.PdfCompliance 枚举。指定输出文件的 PDF 合规级别"
type: docs
weight: 2070
url: /zh/net/aspose.tasks.saving/pdfcompliance/
---
## PdfCompliance enumeration

指定输出文件的 PDF 合规级别。

```csharp
public enum PdfCompliance
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| Pdf15 | `0` | PDF/15 合规级别。 |
| PdfA1a | `1` | PDF/A-1a 合规级别。 |
| PdfA1b | `2` | PDF/A-1b 合规级别。 |

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

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


