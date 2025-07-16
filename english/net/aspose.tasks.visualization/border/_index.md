---
title: Enum Border
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.Visualization.Border enum. Specifies the type borders
type: docs
weight: 2890
url: /net/aspose.tasks.visualization/border/
---
## Border enumeration

Specifies the type borders.

```csharp
public enum Border
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| NoBorder | `0` | No border. |
| AroundEveryPage | `1` | Around every page. |
| OutsidePages | `2` | On the outside pages. |

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


