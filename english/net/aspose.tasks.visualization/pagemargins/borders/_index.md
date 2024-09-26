---
title: PageMargins.Borders
second_title: Aspose.Tasks for .NET API Reference
description: PageMargins property. Gets or sets a position where to print borders. Can be one of the values of the Border enumeration
type: docs
weight: 20
url: /net/aspose.tasks.visualization/pagemargins/borders/
---
## PageMargins.Borders property

Gets or sets a position where to print borders. Can be one of the values of the [`Border`](../../border/) enumeration.

```csharp
public Border Borders { get; set; }
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

* enum [Border](../../border/)
* class [PageMargins](../)
* namespace [Aspose.Tasks.Visualization](../../pagemargins/)
* assembly [Aspose.Tasks](../../../)


