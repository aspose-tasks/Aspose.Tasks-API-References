---
title: Class PageMargins
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.Visualization.PageMargins class. Represents page margins for printing
type: docs
weight: 3210
url: /net/aspose.tasks.visualization/pagemargins/
---
## PageMargins class

Represents page margins for printing.

```csharp
public class PageMargins
```

## Constructors

| Name | Description |
| --- | --- |
| [PageMargins](pagemargins/)() | The default constructor. |

## Properties

| Name | Description |
| --- | --- |
| [Borders](../../aspose.tasks.visualization/pagemargins/borders/) { get; set; } | Gets or sets a position where to print borders. Can be one of the values of the [`Border`](../border/) enumeration. |
| [Bottom](../../aspose.tasks.visualization/pagemargins/bottom/) { get; set; } | Gets or sets the size of the bottom margin in centimeters. |
| [Left](../../aspose.tasks.visualization/pagemargins/left/) { get; set; } | Gets or sets the size of the left margin in centimeters. |
| [Right](../../aspose.tasks.visualization/pagemargins/right/) { get; set; } | Gets or sets the size of the right margin in centimeters. |
| [Top](../../aspose.tasks.visualization/pagemargins/top/) { get; set; } | Gets or sets the size of the top margin in centimeters. |

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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


