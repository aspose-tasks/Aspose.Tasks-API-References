---
title: ProjectView.GetDefaultResourceUsageView
second_title: Aspose.Tasks for .NET API Reference
description: ProjectView method. Includes Uid name start finish and work resource columns
type: docs
weight: 50
url: /net/aspose.tasks.visualization/projectview/getdefaultresourceusageview/
---
## ProjectView.GetDefaultResourceUsageView method

Includes Uid, name, start, finish and work resource columns.

```csharp
public static ProjectView GetDefaultResourceUsageView()
```

### Return Value

a view which contains a list of [`ResourceViewColumn`](../../resourceviewcolumn/).

## Examples

Shows how to save a project with resource usage view.

```csharp
var project = new Project(DataDir + "Project2.mpp");
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.Months,
    View = ProjectView.GetDefaultResourceUsageView()
};

project.Save(OutDir + "WorkWithProjectView_ResourceUsageView_out.pdf", options);
```

### See Also

* class [ProjectView](../)
* namespace [Aspose.Tasks.Visualization](../../projectview/)
* assembly [Aspose.Tasks](../../../)


