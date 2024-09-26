---
title: HtmlSaveOptions.CssStylePrefix
second_title: Aspose.Tasks for .NET API Reference
description: HtmlSaveOptions property. Gets or sets CSS style prefix
type: docs
weight: 30
url: /net/aspose.tasks.saving/htmlsaveoptions/cssstyleprefix/
---
## HtmlSaveOptions.CssStylePrefix property

Gets or sets CSS style prefix.

```csharp
public string CssStylePrefix { get; set; }
```

## Examples

Shows how to set a common prefix for CSS styles are used during export to HTML.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

var options = new HtmlSaveOptions { CssStylePrefix = "test_prefix" };

project.Save(OutDir + "TestCssStylePrefix_out.html", options);
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../htmlsaveoptions/)
* assembly [Aspose.Tasks](../../../)


