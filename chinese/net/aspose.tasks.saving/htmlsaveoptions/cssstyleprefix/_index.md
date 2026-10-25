---
title: "HtmlSaveOptions.CssStylePrefix"
second_title: "Aspose.Tasks for .NET API 参考"
description: "HtmlSaveOptions 属性。获取或设置 CSS 样式前缀"
type: docs
weight: 30
url: /zh/net/aspose.tasks.saving/htmlsaveoptions/cssstyleprefix/
---
## HtmlSaveOptions.CssStylePrefix property

获取或设置 CSS 样式前缀。

```csharp
public string CssStylePrefix { get; set; }
```

## 示例

展示如何为导出为 HTML 时使用的 CSS 样式设置公共前缀。

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

var options = new HtmlSaveOptions { CssStylePrefix = "test_prefix" };

project.Save(OutDir + "TestCssStylePrefix_out.html", options);
```

### 另见

* class [HtmlSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../htmlsaveoptions/)
* assembly [Aspose.Tasks](../../../)


