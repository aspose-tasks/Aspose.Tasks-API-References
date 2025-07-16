---
title: Enum PresentationFormat
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.Visualization.PresentationFormat enum. Enumeration for presentation format
type: docs
weight: 3190
url: /net/aspose.tasks.visualization/presentationformat/
---
## PresentationFormat enumeration

Enumeration for presentation format.

```csharp
public enum PresentationFormat
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| GanttChart | `0` | Gantt Chart presentation format. |
| TaskUsage | `1` | Task usage presentation format. |
| ResourceUsage | `2` | Resource usage presentation format. |
| ResourceSheet | `3` | Resource sheet presentation format. |
| TaskSheet | `4` | Task sheet presentation format. |

## Examples

Shows how to render resource sheet view.

```csharp
var project = new Project(DataDir + "ResourceSheetView.mpp");

SaveOptions options = new PdfSaveOptions();

// Set the Presentation Format to Resource Sheet
options.PresentationFormat = PresentationFormat.ResourceSheet;
project.Save(OutDir + "ResourceSheetView_out.pdf", options);
```

### See Also

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


