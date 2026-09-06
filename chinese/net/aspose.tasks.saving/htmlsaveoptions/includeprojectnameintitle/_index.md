---
title: "HtmlSaveOptions.IncludeProjectNameInTitle"
second_title: "Aspose.Tasks for .NET API 参考"
description: "HtmlSaveOptions 属性。获取或设置一个值，指示是否在 HTML 标题中包含项目名称。"
type: docs
weight: 120
url: /zh/net/aspose.tasks.saving/htmlsaveoptions/includeprojectnameintitle/
---
## HtmlSaveOptions.IncludeProjectNameInTitle property

获取或设置一个值，指示是否在 HTML 标题中包含项目名称。

```csharp
public bool IncludeProjectNameInTitle { get; set; }
```

## 示例

展示如何使用 &lt;see cref=\"P:Aspose.Tasks.Saving.HtmlSaveOptions\" /&gt; 选项设置页面 HTML 标题/标题。

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
var options = new HtmlSaveOptions
{
    // 确定是否在 HTML 标题中包含项目名称（默认 true）
    IncludeProjectNameInTitle = false,

    // 确定是否在 HTML 页面标题中包含项目名称（默认 true）
    IncludeProjectNameInPageHeader = false,

    // 设置将要导出的页面
    Pages = new List<int>
            {
                1
            }
};
project.Save(OutDir + "ControlHeaderNameDuringHTMLExport_out.html", options);
```

### 另见

* class [HtmlSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../htmlsaveoptions/)
* assembly [Aspose.Tasks](../../../)


