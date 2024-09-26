---
title: TaskUsageViewFieldCollection.GetEnumerator
second_title: Aspose.Tasks for .NET API Reference
description: TaskUsageViewFieldCollection method. Returns an enumerator for this collection
type: docs
weight: 10
url: /net/aspose.tasks/taskusageviewfieldcollection/getenumerator/
---
## TaskUsageViewFieldCollection.GetEnumerator method

Returns an enumerator for this collection.

```csharp
public IEnumerator<TaskUsageViewField> GetEnumerator()
```

### Return Value

an enumerator for this collection.

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


