---
title: HtmlSaveOptions.HtmlSaveOptions
second_title: Aspose.Tasks for .NET API Reference
description: HtmlSaveOptions constructor. Initializes a new instance of the HtmlSaveOptions class
type: docs
weight: 10
url: /net/aspose.tasks.saving/htmlsaveoptions/htmlsaveoptions/
---
## HtmlSaveOptions constructor

Initializes a new instance of the [`HtmlSaveOptions`](../) class.

```csharp
public HtmlSaveOptions()
```

## Examples

Shows how to save a project in HTML format.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
var option = new HtmlSaveOptions();
project.Save(OutDir + "SaveProjectDataAsHTML_out.html", option);

// OR

// Adding only one page (page number 2)
option = new HtmlSaveOptions();
option.Pages.Add(2);
project.Save(OutDir + "SaveProjectDataAsHTML2_out.html", option);
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../htmlsaveoptions/)
* assembly [Aspose.Tasks](../../../)


