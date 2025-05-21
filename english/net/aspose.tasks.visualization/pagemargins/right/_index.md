---
title: PageMargins.Right
second_title: Aspose.Tasks for .NET API Reference
description: PageMargins property. Gets or sets the size of the right margin in centimeters
type: docs
weight: 50
url: /net/aspose.tasks.visualization/pagemargins/right/
---
## PageMargins.Right property

Gets or sets the size of the right margin in centimeters.

```csharp
public double Right { get; set; }
```

## Examples

Shows how to work with page margins.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// lets modify the default view
var margins = project.DefaultView.PageInfo.Margins;

// lets modify margins
margins.Left = 10d;
margins.Top = 10d;
margins.Right = 10d;
margins.Bottom = 10d;
margins.Borders = Border.OutsidePages;

project.Save(OutDir + "WorkWithPageMargins_out.mpp", SaveFileFormat.Mpp);
```

### See Also

* class [PageMargins](../)
* namespace [Aspose.Tasks.Visualization](../../pagemargins/)
* assembly [Aspose.Tasks](../../../)


