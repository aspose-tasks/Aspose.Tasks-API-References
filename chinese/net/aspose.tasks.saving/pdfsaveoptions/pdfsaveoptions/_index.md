---
title: "PdfSaveOptions.PdfSaveOptions"
second_title: "Aspose.Tasks for .NET API 参考"
description: "PdfSaveOptions 构造函数。初始化一个 PdfSaveOptions 类的新实例，可用于将文档保存为 PDF 格式"
type: docs
weight: 10
url: /zh/net/aspose.tasks.saving/pdfsaveoptions/pdfsaveoptions/
---
## PdfSaveOptions constructor

初始化一个 [`PdfSaveOptions`](../) 类的新实例，可用于将文档保存为 [`PDF`](../../savefileformat/) 格式。

```csharp
public PdfSaveOptions()
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


