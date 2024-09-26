---
title: TaskUsageView.FieldCollection
second_title: Aspose.Tasks for .NET API Reference
description: TaskUsageView property. Gets TaskUsageViewFieldCollection object of this TaskUsageView
type: docs
weight: 10
url: /net/aspose.tasks/taskusageview/fieldcollection/
---
## TaskUsageView.FieldCollection property

Gets [`TaskUsageViewFieldCollection`](../../taskusageviewfieldcollection/) object of this TaskUsageView.

```csharp
public TaskUsageViewFieldCollection FieldCollection { get; }
```

## Examples

Shows how to read task usage view fields.

```csharp
var project = new Project(DataDir + "TaskUsageView.mpp");

var view = (TaskUsageView)project.Views.ToList()[2];
foreach (var field in view.FieldCollection)
{
    Console.WriteLine("Field: " + field);
}
```

### See Also

* class [TaskUsageViewFieldCollection](../../taskusageviewfieldcollection/)
* class [TaskUsageView](../)
* namespace [Aspose.Tasks](../../taskusageview/)
* assembly [Aspose.Tasks](../../../)


