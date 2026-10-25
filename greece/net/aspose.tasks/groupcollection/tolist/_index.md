---
title: "GroupCollection.ToList"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος GroupCollection. Μετατρέπει μια συλλογή ομάδων σε λίστα αντικειμένων Group"
type: docs
weight: 90
url: /el/net/aspose.tasks/groupcollection/tolist/
---
## GroupCollection.ToList method

Μετατρέπει μια συλλογή ομάδων σε λίστα αντικειμένων [`Group`](../../group/).

```csharp
public List<Group> ToList()
```

### Τιμή Επιστροφής

Γενική λίστα αντικειμένων [`Group`](../../group/).

## Παραδείγματα

Δείχνει πώς να εργαστείτε με μια συλλογή ομάδων.

```csharp
var project = new Project(DataDir + "ReadGroupDefinitionData.mpp");

// επανάληψη στις ομάδες εργασιών
Console.WriteLine("Print task groups of {0} project: ", project.Get(Prj.Name));
Console.WriteLine("Task Group Count: " + project.TaskGroups.Count);
foreach (var group in project.TaskGroups)
{
    Console.WriteLine("Name: " + group.Name);
    Console.WriteLine("Show In Menu: " + group.ShowInMenu);
    Console.WriteLine();
}

// επανάληψη στις ομάδες πόρων
Console.WriteLine("Project resource group count: " + project.ResourceGroups.Count);
foreach (var group in project.ResourceGroups)
{
    Console.WriteLine("Resource group Name: " + group.Name);
    Console.WriteLine("Resource group ShowInMenu" + group.ShowInMenu);
}

var otherProject = new Project(DataDir + "Blank2010.mpp");

// καθαρισμός των ομάδων του άλλου έργου
otherProject.TaskGroups.Clear();

// αντιγραφή ομάδων σε άλλο έργο
var groups = new Group[project.TaskGroups.Count];
project.TaskGroups.CopyTo(groups, 0);

foreach (var group in groups)
{
    otherProject.TaskGroups.Add(group);
}

// προσθήκη προσαρμοσμένης ομάδας εργασιών
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

// αφαίρεση όλων των ομάδων
List<Group> groupsToDelete = otherProject.TaskGroups.ToList();
foreach (var group in groupsToDelete)
{
    otherProject.TaskGroups.Remove(group);
}
```

### Δείτε επίσης

* class [Group](../../group/)
* class [GroupCollection](../)
* namespace [Aspose.Tasks](../../groupcollection/)
* assembly [Aspose.Tasks](../../../)


