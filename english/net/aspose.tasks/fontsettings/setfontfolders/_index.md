---
title: FontSettings.SetFontFolders
second_title: Aspose.Tasks for .NET API Reference
description: FontSettings method. Sets the folders where Aspose.Tasks looks for TrueType fonts when rendering projects view
type: docs
weight: 50
url: /net/aspose.tasks/fontsettings/setfontfolders/
---
## FontSettings.SetFontFolders method

Sets the folders where Aspose.Tasks looks for TrueType fonts when rendering project's view.

```csharp
public void SetFontFolders(string[] fontFolders, bool recursive)
```

| Parameter | Type | Description |
| --- | --- | --- |
| fontFolders | String[] | An array of folders that contain TrueType fonts. |
| recursive | Boolean | If true the specified folders will be scanned recursively. |

## Examples

Shows how to set custom font folder.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions
{
    PresentationFormat = PresentationFormat.GanttChart,
};

// TrueType font files for all fonts used in the opened project should be located in MyFonts folder.
options.FontSettings.SetFontFolders(new string[] { "c:\\MyFonts"}, true);

project.Save(OutDir + "EstimatedMilestoneTasks_out4.pdf", options);
```

### See Also

* class [FontSettings](../)
* namespace [Aspose.Tasks](../../fontsettings/)
* assembly [Aspose.Tasks](../../../)


