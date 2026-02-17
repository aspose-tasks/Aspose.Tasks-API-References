---
title: Class GroupCollection
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.GroupCollection class. Contains a list of Group objects. Implements ICollectionGroup interface
type: docs
weight: 780
url: /net/aspose.tasks/groupcollection/
---
## GroupCollection class

Contains a list of [`Group`](../group/) objects. Implements ICollection&lt;Group&gt; interface.

```csharp
public class GroupCollection : ICollection<Group>
```

## Properties

| Name | Description |
| --- | --- |
| [Count](../../aspose.tasks/groupcollection/count/) { get; } | Gets the number of elements contained in this collection. |
| [IsReadOnly](../../aspose.tasks/groupcollection/isreadonly/) { get; } | Gets a value indicating whether this collection is read-only. |

## Methods

| Name | Description |
| --- | --- |
| [Add](../../aspose.tasks/groupcollection/add/)(Group) | Adds the specified item to this collection. |
| [Clear](../../aspose.tasks/groupcollection/clear/)() | Removes all items from this collection. |
| [Contains](../../aspose.tasks/groupcollection/contains/)(Group) | Returns true if the specified item is found in this collection; otherwise, false. |
| [CopyTo](../../aspose.tasks/groupcollection/copyto/)(Group[], int) | Copies the elements of this collection to the specified array, starting at the specified array index. |
| [GetEnumerator](../../aspose.tasks/groupcollection/getenumerator/)() | Returns an enumerator for this collection. |
| [Remove](../../aspose.tasks/groupcollection/remove/)(Group) | Removes the first occurrence of a specific object from this collection. |
| [ToList](../../aspose.tasks/groupcollection/tolist/)() | Converts a group collection to a list of [`Group`](../group/) objects. |

## Examples

Shows how to work with collection of groups.

```csharp
var project = new Project(DataDir + "ReadGroupDefinitionData.mpp");

// iterate over task groups
Console.WriteLine("Print task groups of {0} project: ", project.Get(Prj.Name));
Console.WriteLine("Task Group Count: " + project.TaskGroups.Count);
foreach (var group in project.TaskGroups)
{
    Console.WriteLine("Name: " + group.Name);
    Console.WriteLine("Show In Menu: " + group.ShowInMenu);
    Console.WriteLine();
}

// iterate over resource groups
Console.WriteLine("Project resource group count: " + project.ResourceGroups.Count);
foreach (var group in project.ResourceGroups)
{
    Console.WriteLine("Resource group Name: " + group.Name);
    Console.WriteLine("Resource group ShowInMenu" + group.ShowInMenu);
}

var otherProject = new Project(DataDir + "Blank2010.mpp");

// clear other project's groups
otherProject.TaskGroups.Clear();

// copy groups to other project
var groups = new Group[project.TaskGroups.Count];
project.TaskGroups.CopyTo(groups, 0);

foreach (var group in groups)
{
    otherProject.TaskGroups.Add(group);
}

// add custom task group
var customGroup = new Group
{
    Name = "Custom Group",
    ShowInMenu = true
};

if (!otherProject.TaskGroups.Contains(customGroup))
{
    if (!otherProject.TaskGroups.IsReadOnly)
    {
        otherProject.TaskGroups.Add(customGroup);
    }
}

// remove all groups
List<Group> groupsToDelete = otherProject.TaskGroups.ToList();
foreach (var group in groupsToDelete)
{
    otherProject.TaskGroups.Remove(group);
}
```

### See Also

* class [Group](../group/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


