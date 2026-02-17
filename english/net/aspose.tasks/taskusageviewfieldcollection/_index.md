---
title: Class TaskUsageViewFieldCollection
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.TaskUsageViewFieldCollection class. Represents a collection of TaskUsageViewField values
type: docs
weight: 2480
url: /net/aspose.tasks/taskusageviewfieldcollection/
---
## TaskUsageViewFieldCollection class

Represents a collection of [`TaskUsageViewField`](../taskusageviewfield/) values.

```csharp
public class TaskUsageViewFieldCollection : IList<TaskUsageViewField>
```

## Methods

| Name | Description |
| --- | --- |
| [GetEnumerator](../../aspose.tasks/taskusageviewfieldcollection/getenumerator/)() | Returns an enumerator for this collection. |
| [ToList](../../aspose.tasks/taskusageviewfieldcollection/tolist/)() | Returns a list which contains all items from this collection. |

## Examples

Shows how to work field collection of a TaskUsageView instance.

```csharp
var project = new Project(DataDir + "TaskUsageView.mpp");

var view = (TaskUsageView)project.Views.ToList()[2];
foreach (var field in view.FieldCollection)
{
    Console.WriteLine("Field: " + field);
}

// one can transform collection into a list of TaskUsageViewField
IList<TaskUsageViewField> fields = view.FieldCollection.ToList();
foreach (var field in fields)
{
    Console.WriteLine("Field (from the list): " + field);
}
```

### See Also

* enum [TaskUsageViewField](../taskusageviewfield/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


