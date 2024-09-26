---
title: TaskUsageViewFieldCollection.ToList
second_title: Aspose.Tasks for .NET API Reference
description: TaskUsageViewFieldCollection method. Returns a list which contains all items from this collection
type: docs
weight: 20
url: /net/aspose.tasks/taskusageviewfieldcollection/tolist/
---
## TaskUsageViewFieldCollection.ToList method

Returns a list which contains all items from this collection.

```csharp
public IList<TaskUsageViewField> ToList()
```

### Return Value

returns a list which contains all items from this collection.

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

* enum [TaskUsageViewField](../../taskusageviewfield/)
* class [TaskUsageViewFieldCollection](../)
* namespace [Aspose.Tasks](../../taskusageviewfieldcollection/)
* assembly [Aspose.Tasks](../../../)


