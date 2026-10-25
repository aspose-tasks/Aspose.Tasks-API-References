---
title: "SaveOptions.PageCount"
second_title: "Aspose.Tasks for .NET API 参考"
description: "SaveOptions 属性。获取或设置项目的页数。"
type: docs
weight: 120
url: /zh/net/aspose.tasks.saving/saveoptions/pagecount/
---
## SaveOptions.PageCount property

获取或设置项目的页数。

```csharp
public int PageCount { get; }
```

## 示例

展示如何将项目的选定页面保存为 PDF 文件。

```csharp
var project = new Project(DataDir + "Software Development Plan.mpp");
var options = new PdfSaveOptions();
options.RenderToSinglePage = false;
options.Pages = new List<int>();

// 让我们检查可以导出的页面数量
Console.WriteLine("Page Count: " + options.PageCount);

options.Pages.Add(1);
options.Pages.Add(4);
project.Save(OutDir + "SaveToMultiplePDFFiles_out.pdf", options);
```

### 另见

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


