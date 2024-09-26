---
title: HtmlSaveOptions.IncludeProjectNameInTitle
second_title: Aspose.Tasks for .NET API Reference
description: HtmlSaveOptions property. Gets or sets a value indicating whether to include project name in HTML title
type: docs
weight: 120
url: /net/aspose.tasks.saving/htmlsaveoptions/includeprojectnameintitle/
---
## HtmlSaveOptions.IncludeProjectNameInTitle property

Gets or sets a value indicating whether to include project name in HTML title.

```csharp
public bool IncludeProjectNameInTitle { get; set; }
```

## Examples

Shows how to set page HTML header/title by using &lt;see cref="P:Aspose.Tasks.Saving.HtmlSaveOptions" /&gt; options.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
var options = new HtmlSaveOptions
{
    // Determines whether to include project name in HTML title (true by default)
    IncludeProjectNameInTitle = false,

    // Determines whether to include project name in HTML page header  (true by default)
    IncludeProjectNameInPageHeader = false,

    // set pages that will be exported
    Pages = new List<int>
            {
                1
            }
};
project.Save(OutDir + "ControlHeaderNameDuringHTMLExport_out.html", options);
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../htmlsaveoptions/)
* assembly [Aspose.Tasks](../../../)


