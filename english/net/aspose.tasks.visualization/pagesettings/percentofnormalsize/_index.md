---
title: PageSettings.PercentOfNormalSize
second_title: Aspose.Tasks for .NET API Reference
description: PageSettings property. Gets or sets a percentage of normal size to adjust printing to
type: docs
weight: 90
url: /net/aspose.tasks.visualization/pagesettings/percentofnormalsize/
---
## PageSettings.PercentOfNormalSize property

Gets or sets a percentage of normal size to adjust printing to.

```csharp
public int PercentOfNormalSize { get; set; }
```

## Examples

Shows how to render view with the specified scale factor.

```csharp
var project = new Project(DataDir + "Input.mpp");

var view = project.Views.First(v => v.Screen == ViewScreen.Gantt);

// set a value indicating that view should be scaled using the specified scale factor
view.PageInfo.PageSettings.AdjustToPercentOfNormalSize = true;
// specify the scale factor
view.PageInfo.PageSettings.PercentOfNormalSize = 33;

PdfSaveOptions saveOptions = new PdfSaveOptions()
{
    ViewSettings = view,
    Timescale = Timescale.DefinedInView
};

project.Save(OutDir + "PrintViewWithSpecifiedScaleFactor_out.pdf", saveOptions);
```

### See Also

* class [PageSettings](../)
* namespace [Aspose.Tasks.Visualization](../../pagesettings/)
* assembly [Aspose.Tasks](../../../)


