---
title: ProjectView.GetDefaultAssignmentView
second_title: Aspose.Tasks for .NET API Reference
description: ProjectView method. Includes Uid task name resource name work and duration assignment columns
type: docs
weight: 20
url: /net/aspose.tasks.visualization/projectview/getdefaultassignmentview/
---
## ProjectView.GetDefaultAssignmentView method

Includes Uid, task name, resource name, work and duration assignment columns.

```csharp
public static ProjectView GetDefaultAssignmentView()
```

### Return Value

a view which contains a list of [`AssignmentViewColumn`](../../assignmentviewcolumn/).

## Examples

Shows how to save a project with assignment view.

```csharp
var project = new Project(DataDir + "Project2.mpp");
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.Months,
    View = ProjectView.GetDefaultAssignmentView()
};

project.Save(OutDir + "WorkWithProjectView_AssignmentView_out.pdf", options);
```

### See Also

* class [ProjectView](../)
* namespace [Aspose.Tasks.Visualization](../../projectview/)
* assembly [Aspose.Tasks](../../../)


