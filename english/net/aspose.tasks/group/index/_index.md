---
title: Group.Index
second_title: Aspose.Tasks for .NET API Reference
description: Group property. Gets the index of a Group object in the Groups containing object
type: docs
weight: 40
url: /net/aspose.tasks/group/index/
---
## Group.Index property

Gets the index of a [`Group`](../) object in the Groups containing object.

```csharp
public int Index { get; }
```

## Examples

Shows how to work with groups.

```csharp
var project = new Project(DataDir + "ReadGroupDefinitionData.mpp");

Console.WriteLine("Task Groups Count: " + project.TaskGroups.Count);
var group = project.TaskGroups.ToList()[1];
Console.WriteLine("Task Group Uid: " + group.Uid);
Console.WriteLine("Task Group Index: " + group.Index);
Console.WriteLine("Task Group Name: " + group.Name);
Console.WriteLine("Is Task Group Maintain Hierarchy?: " + group.MaintainHierarchy);
Console.WriteLine("Is Task Group Show In Menu?: " + group.ShowInMenu);
Console.WriteLine("Is Task Group Show Summary?: " + group.ShowSummary);
Console.WriteLine("Is Task Group should groups Assignments instead of Tasks?: " + group.GroupAssignments);
Console.WriteLine("Task Group Criteria count: " + group.GroupCriteria.Count);
Console.WriteLine("\n************* Retrieving Task Group's Criterion information *************");

foreach (var criterion in group.GroupCriteria)
{
    Console.WriteLine("Task Criterion Field: " + criterion.Field);
    Console.WriteLine("Task Criterion GroupOn: " + criterion.GroupOn);
    Console.WriteLine("Task Criterion Cell Color: " + criterion.CellColor);
    Console.WriteLine("Task Criterion Pattern: " + criterion.Pattern);

    if (group == criterion.ParentGroup)
    {
        Console.WriteLine("Parent Group is equal to task Group.");
    }

    Console.WriteLine("Font Name: " + criterion.Font.FontFamily);
    Console.WriteLine("Font Size: " + criterion.Font.Size);
    Console.WriteLine("Font Style: " + criterion.Font.Style);
    Console.WriteLine("Ascending/Descending: " + criterion.Ascending);
}
```

### See Also

* class [Group](../)
* namespace [Aspose.Tasks](../../group/)
* assembly [Aspose.Tasks](../../../)


