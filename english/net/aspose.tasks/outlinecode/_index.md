---
title: Class OutlineCode
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.OutlineCode class. Represents a value of an outline code
type: docs
weight: 1130
url: /net/aspose.tasks/outlinecode/
---
## OutlineCode class

Represents a value of an outline code.

```csharp
public class OutlineCode
```

## Constructors

| Name | Description |
| --- | --- |
| [OutlineCode](outlinecode/#constructor)() | Initializes a new instance of the `OutlineCode` class. |
| [OutlineCode](outlinecode/#constructor_1)(OutlineCodeDefinition, OutlineValue) | Initializes a new instance of the `OutlineCode` class using the specified Outline Code and one of its values. |

## Properties

| Name | Description |
| --- | --- |
| [FieldId](../../aspose.tasks/outlinecode/fieldid/) { get; set; } | Gets or sets the number value of the project Id custom field. |
| [ValueGuid](../../aspose.tasks/outlinecode/valueguid/) { get; set; } | Gets or sets the GUID of the value in the value list. The ValueGuid matches the FieldGuid in the value list. |
| [ValueId](../../aspose.tasks/outlinecode/valueid/) { get; set; } | Gets or sets the Id in the value list associated with the definition in the outline code collection. |

## Remarks

Two pieces of data are necessary - a pointer to the outline code table that is specified by the FieldId, and the value that is specified either by the ValueId or ValueGuid pointer to the value list.

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


