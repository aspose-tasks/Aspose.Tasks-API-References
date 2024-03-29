---
title: FontResolveCallback
second_title: Aspose.Tasks for .NET API Reference
description: Gets or sets a callback which can be used to customize resolved fonts.
type: docs
weight: 90
url: /net/aspose.tasks.saving/htmlsaveoptions/fontresolvecallback/
---
## HtmlSaveOptions.FontResolveCallback property

Gets or sets a callback which can be used to customize resolved fonts.

```csharp
public FontResolveCallbackDelegate FontResolveCallback { get; set; }
```

### Examples

Shows how to set custom font resolve callback to execute user-defined code to set fallback font or to substitute the specific font.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions
{
    PresentationFormat = PresentationFormat.GanttChart,
    FontResolveCallback = delegate(FontResolveEventArgs args)
    {
        if (args.RequestedFontName != args.ResolvedFontName)
        {
            // Looks like the exact font cannot be found and fallback font was set.
            // We can override the fallback font.
            args.ResolvedFontName = "Arial";
        }

        // Or simply substitute the specific font:
        if (args.RequestedFontName == "Comic Sans MS")
        {
            args.ResolvedFontName = "Arial";
        }
    }
};

project.Save(OutDir + "EstimatedMilestoneTasks_out3.pdf", options);
```

### See Also

* delegate [FontResolveCallbackDelegate](../../../aspose.tasks/fontresolvecallbackdelegate)
* class [HtmlSaveOptions](../../htmlsaveoptions)
* namespace [Aspose.Tasks.Saving](../../htmlsaveoptions)
* assembly [Aspose.Tasks](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
