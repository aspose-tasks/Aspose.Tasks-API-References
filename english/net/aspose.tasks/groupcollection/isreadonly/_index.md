---
title: GroupCollection.IsReadOnly
second_title: Aspose.Tasks for .NET API Reference
description: GroupCollection property. Gets a value indicating whether this collection is readonly
type: docs
weight: 20
url: /net/aspose.tasks/groupcollection/isreadonly/
---
## GroupCollection.IsReadOnly property

Gets a value indicating whether this collection is read-only.

```csharp
public bool IsReadOnly { get; }
```

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

* class [GroupCollection](../)
* namespace [Aspose.Tasks](../../groupcollection/)
* assembly [Aspose.Tasks](../../../)


