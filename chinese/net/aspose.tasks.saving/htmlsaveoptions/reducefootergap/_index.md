---
title: "HtmlSaveOptions.ReduceFooterGap"
second_title: "Aspose.Tasks for .NET API 参考"
description: "HtmlSaveOptions 属性。获取或设置一个值，指示是否需要缩小最后任务与页脚之间的间距。"
type: docs
weight: 150
url: /zh/net/aspose.tasks.saving/htmlsaveoptions/reducefootergap/
---
## HtmlSaveOptions.ReduceFooterGap property

获取或设置一个值，指示是否必须缩小最后任务与页脚之间的间距。

```csharp
public bool ReduceFooterGap { get; set; }
```

## 示例

展示如何在 HTML 输出文件中设置一个值，以指示是否需要缩小最后任务与页脚之间的间距。

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new HtmlSaveOptions
                  {
                      ReduceFooterGap = true,
                      IncludeProjectNameInPageHeader = false,
                      IncludeProjectNameInTitle = false,
                      PageSize = PageSize.A0,
                      Timescale = Timescale.Days
                  };
project.Save(OutDir + "ReducingGapBetweenTasksListAndFooter_out.html", options);
```

### 另见

* class [HtmlSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../htmlsaveoptions/)
* assembly [Aspose.Tasks](../../../)


