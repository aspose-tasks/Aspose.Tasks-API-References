---
title: "ImageSaveOptions.ReduceFooterGap"
second_title: "Aspose.Tasks for .NET API 参考"
description: "ImageSaveOptions 属性。获取或设置一个值，指示是否需要缩小最后任务与页脚之间的间距"
type: docs
weight: 80
url: /zh/net/aspose.tasks.saving/imagesaveoptions/reducefootergap/
---
## ImageSaveOptions.ReduceFooterGap property

获取或设置一个值，指示是否必须缩小最后任务与页脚之间的间距。

```csharp
public bool ReduceFooterGap { get; set; }
```

## 示例

展示如何设置指示是否需要缩小最后任务与页脚之间间距的值。

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

// 使用 ReduceFooterGap 属性来缩小任务列表与页脚之间的间距
var imageSaveOptions = new ImageSaveOptions(SaveFileFormat.Png)
                           {
                               ReduceFooterGap = true, /* set to true */ 
                               RenderToSinglePage = false,
                               PageSize = PageSize.A0,
                               Timescale = Timescale.Days
                           };
project.Save(OutDir + "ReducingGapBetweenTasksListAndFooter_out.png", imageSaveOptions);
```

### 另见

* class [ImageSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../imagesaveoptions/)
* assembly [Aspose.Tasks](../../../)


