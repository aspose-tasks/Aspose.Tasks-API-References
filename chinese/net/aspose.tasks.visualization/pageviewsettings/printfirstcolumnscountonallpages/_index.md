---
title: "PageViewSettings.PrintFirstColumnsCountOnAllPages"
second_title: "Aspose.Tasks for .NET API 参考"
description: "PageViewSettings 属性。获取或设置一个值，指示是否在所有页面上打印指定数量的首列"
type: docs
weight: 60
url: /zh/net/aspose.tasks.visualization/pageviewsettings/printfirstcolumnscountonallpages/
---
## PageViewSettings.PrintFirstColumnsCountOnAllPages property

获取或设置一个值，指示是否在所有页面上打印指定数量的首列。

```csharp
public bool PrintFirstColumnsCountOnAllPages { get; set; }
```

## 示例

展示如何在单独的页面上打印任务、资源、分配备注。

```csharp
var project = new Project(DataDir + "Input.mpp");

// 设置所有页面上要打印的首列数量
project.DefaultView.PageInfo.PageViewSettings.FirstColumnsCount = 2;

// 设置一个值，指示是否打印备注。
project.DefaultView.PageInfo.PageViewSettings.PrintNotes = true;

// 设置一个值，指示在打印时是否将时间尺度适配到页面末尾。
project.DefaultView.PageInfo.PageViewSettings.FitTimescaleToEndOfPage = true;

// 设置一个值，指示是否打印视图的所有工作表列
project.DefaultView.PageInfo.PageViewSettings.PrintAllSheetColumns = true;

// 设置一个值，指示是否打印视图的空白页
project.DefaultView.PageInfo.PageViewSettings.PrintBlankPages = false;

// 设置一个值，指示是否在所有页面上打印指定数量的首列
project.DefaultView.PageInfo.PageViewSettings.PrintFirstColumnsCountOnAllPages = true;

project.Save(OutDir + "ProjectWithComments_out.pdf", SaveFileFormat.Pdf);
```

### 另见

* class [PageViewSettings](../)
* namespace [Aspose.Tasks.Visualization](../../pageviewsettings/)
* assembly [Aspose.Tasks](../../../)


