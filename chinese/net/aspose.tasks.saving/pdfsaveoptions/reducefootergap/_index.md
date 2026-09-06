---
title: "PdfSaveOptions.ReduceFooterGap"
second_title: "Aspose.Tasks for .NET API 参考"
description: "PdfSaveOptions 属性。获取或设置指示是否必须减少最后任务与页脚之间间距的值。"
type: docs
weight: 80
url: /zh/net/aspose.tasks.saving/pdfsaveoptions/reducefootergap/
---
## PdfSaveOptions.ReduceFooterGap property

获取或设置一个值，指示是否必须缩小最后任务与页脚之间的间距。

```csharp
public bool ReduceFooterGap { get; set; }
```

## 示例

展示如何在 PDF 输出文件中设置指示是否必须减少最后任务与页脚之间间距的值。

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions { ReduceFooterGap = true, PageSize = PageSize.A0, Timescale = Timescale.Days };

project.Save(OutDir + "ReducingGapBetweenTasksListAndFooter_out.pdf", options);
```

### 另见

* class [PdfSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../pdfsaveoptions/)
* assembly [Aspose.Tasks](../../../)


