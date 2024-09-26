---
title: ProjectView.GetDefaultResourceSheetView
second_title: Aspose.Tasks for .NET API Reference
description: ProjectView method. Includes Uid resource name type material label initials group max units standard rate overtime rate cost per use accrue at base calendar and code resource columns
type: docs
weight: 40
url: /net/aspose.tasks.visualization/projectview/getdefaultresourcesheetview/
---
## ProjectView.GetDefaultResourceSheetView method

Includes Uid, resource name, type, material label, initials, group, max units, standard rate, overtime rate, cost per use, accrue at, base calendar and code resource columns.

```csharp
public static ProjectView GetDefaultResourceSheetView()
```

### Return Value

a view which contains a list of [`ResourceViewColumn`](../../resourceviewcolumn/).

## Examples

Shows how to save a project with resource sheet view.

```csharp
var project = new Project(DataDir + "Project2.mpp");
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.Months,
    View = ProjectView.GetDefaultResourceSheetView()
};

project.Save(OutDir + "WorkWithProjectView_ResourceSheetView_out.pdf", options);
```

### See Also

* class [ProjectView](../)
* namespace [Aspose.Tasks.Visualization](../../projectview/)
* assembly [Aspose.Tasks](../../../)


