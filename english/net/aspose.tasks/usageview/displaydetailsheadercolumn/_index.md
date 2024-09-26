---
title: UsageView.DisplayDetailsHeaderColumn
second_title: Aspose.Tasks for .NET API Reference
description: UsageView property. Gets or sets a value indicating whether to display details header column in the view or not
type: docs
weight: 30
url: /net/aspose.tasks/usageview/displaydetailsheadercolumn/
---
## UsageView.DisplayDetailsHeaderColumn property

Gets or sets a value indicating whether to display details header column in the view or not.

```csharp
public bool DisplayDetailsHeaderColumn { get; set; }
```

## Examples

Shows how to render task usage view with details.

```csharp
var project = new Project(DataDir + "TaskUsageViewWithDetails.mpp");

// get the view
UsageView view = (TaskUsageView)project.DefaultView;

// details header column will not be displayed
view.DisplayDetailsHeaderColumn = false;
view.RepeatDetailsHeaderOnAllRows = false;
view.DisplayShortDetailHeaderNames = false;
view.AlignDetailsData = HorizontalStringAlignment.Near;
project.Save(OutDir + "task usage1_out.pdf", SaveFileFormat.Pdf);

// display details header column
view.DisplayDetailsHeaderColumn = true;

// repeat details header on all assignments rows
view.RepeatDetailsHeaderOnAllRows = true;
view.AlignDetailsData = HorizontalStringAlignment.Far;
project.Save(OutDir + "task usage2_out.pdf", SaveFileFormat.Pdf);
```

### See Also

* class [UsageView](../)
* namespace [Aspose.Tasks](../../usageview/)
* assembly [Aspose.Tasks](../../../)


