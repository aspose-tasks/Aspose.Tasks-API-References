---
title: PageSettings.PagesInHeight
second_title: Aspose.Tasks for .NET API Reference
description: PageSettings property. Gets or sets a number of pages in height to be printed
type: docs
weight: 50
url: /net/aspose.tasks.visualization/pagesettings/pagesinheight/
---
## PageSettings.PagesInHeight property

Gets or sets a number of pages in height to be printed.

```csharp
public int PagesInHeight { get; set; }
```

## Examples

Shows how to render view with 'Fit X to Y pages' option.

```csharp
var project = new Project(DataDir + "TaskUsageView.mpp");

var view = project.Views.First(v => v.Screen == ViewScreen.TaskUsage);

view.PageInfo.PageSettings.AdjustToPercentOfNormalSize = false;
// specify that view should be rendered in 2 pages or less in height
view.PageInfo.PageSettings.PagesInHeight = 2;
// specify that view should be rendered in 1 page in width
view.PageInfo.PageSettings.PagesInWidth = 1;

PdfSaveOptions saveOptions = new PdfSaveOptions()
{
    ViewSettings = view,
    Timescale = Timescale.DefinedInView,
    StartDate =  new DateTime(2000, 04, 1),
    EndDate = new DateTime(2000, 12, 31)
};

project.Save(OutDir + "PrintViewWithFitToPages_out.pdf", saveOptions);
```

### See Also

* class [PageSettings](../)
* namespace [Aspose.Tasks.Visualization](../../pagesettings/)
* assembly [Aspose.Tasks](../../../)


