---
title: GroupCollection.CopyTo
second_title: Aspose.Tasks for .NET API Reference
description: GroupCollection method. Copies the elements of this collection to the specified array starting at the specified array index
type: docs
weight: 60
url: /net/aspose.tasks/groupcollection/copyto/
---
## GroupCollection.CopyTo method

Copies the elements of this collection to the specified array, starting at the specified array index.

```csharp
public void CopyTo(Group[] array, int arrayIndex)
```

| Parameter | Type | Description |
| --- | --- | --- |
| array | Group[] | the specified one-dimensional array to copy elements to |
| arrayIndex | Int32 | the zero-based index of the specified array at which copying begins. |

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

* class [Group](../../group/)
* class [GroupCollection](../)
* namespace [Aspose.Tasks](../../groupcollection/)
* assembly [Aspose.Tasks](../../../)


