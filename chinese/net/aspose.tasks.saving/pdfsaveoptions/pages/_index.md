---
title: "PdfSaveOptions.Pages"
second_title: "Aspose.Tasks for .NET API 参考"
description: "PdfSaveOptions 属性。获取或设置在将项目布局保存为单独文件时要保存的页面编号列表。如果此列表为空，将保存所有页面。"
type: docs
weight: 60
url: /zh/net/aspose.tasks.saving/pdfsaveoptions/pages/
---
## PdfSaveOptions.Pages property

获取或设置在将项目布局保存为单独文件时要保存的页码列表。如果此列表为空，则会保存所有页面。

```csharp
public List<int> Pages { get; set; }
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

* class [PdfSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../pdfsaveoptions/)
* assembly [Aspose.Tasks](../../../)


