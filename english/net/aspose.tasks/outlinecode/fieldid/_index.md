---
title: OutlineCode.FieldId
second_title: Aspose.Tasks for .NET API Reference
description: OutlineCode property. Gets or sets the number value of the project Id custom field
type: docs
weight: 20
url: /net/aspose.tasks/outlinecode/fieldid/
---
## OutlineCode.FieldId property

Gets or sets the number value of the project Id custom field.

```csharp
public string FieldId { get; set; }
```

## Examples

Shows how to read task's outline codes.

```csharp
var project = new Project(DataDir + "OutlineValues2010.mpp");

// read outline codes
foreach (var task in project.RootTask.SelectAllChildTasks())
{
    if (task.OutlineCodes.Count <= 0)
    {
        continue;
    }

    Console.WriteLine("Print outline codes of the task: " + task.Get(Tsk.Name));
    foreach (var value in task.OutlineCodes)
    {
        Console.WriteLine("  Field Id: " + value.FieldId);
        Console.WriteLine("  Value Guid: " + value.ValueGuid);
        Console.WriteLine("  Value Id: " + value.ValueId);
    }
}
```

### See Also

* class [OutlineCode](../)
* namespace [Aspose.Tasks](../../outlinecode/)
* assembly [Aspose.Tasks](../../../)


