---
title: "HtmlSaveOptions.HtmlSaveOptions"
second_title: "Aspose.Tasks for .NET API 参考"
description: "HtmlSaveOptions 构造函数。初始化 HtmlSaveOptions 类的新实例"
type: docs
weight: 10
url: /zh/net/aspose.tasks.saving/htmlsaveoptions/htmlsaveoptions/
---
## HtmlSaveOptions constructor

初始化 [`HtmlSaveOptions`](../) 类的新实例。

```csharp
public HtmlSaveOptions()
```

## 示例

展示如何将项目保存为 HTML 格式。

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
var option = new HtmlSaveOptions();
project.Save(OutDir + "SaveProjectDataAsHTML_out.html", option);

// 或

// 仅添加一页（第 2 页）
option = new HtmlSaveOptions();
option.Pages.Add(2);
project.Save(OutDir + "SaveProjectDataAsHTML2_out.html", option);
```

### 另见

* class [HtmlSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../htmlsaveoptions/)
* assembly [Aspose.Tasks](../../../)


