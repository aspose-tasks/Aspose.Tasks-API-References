---
title: "GroupCollection.Remove"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "GroupCollection‑methode. Verwijdert de eerste voorkoming van een specifiek object uit deze collectie"
type: docs
weight: 80
url: /nl/net/aspose.tasks/groupcollection/remove/
---
## GroupCollection.Remove method

Verwijdert de eerste instantie van een specifiek object uit deze collectie.

```csharp
public bool Remove(Group item)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| item | Group | het opgegeven object om te verwijderen. |

### Retourwaarde

true als het opgegeven object succesvol uit deze collectie is verwijderd; anders false.

## Voorbeelden

Toont hoe te werken met een collectie van groepen.

```csharp
var project = new Project(DataDir + "ReadGroupDefinitionData.mpp");

// itereren over taakgroepen
Console.WriteLine("Print task groups of {0} project: ", project.Get(Prj.Name));
Console.WriteLine("Task Group Count: " + project.TaskGroups.Count);
foreach (var group in project.TaskGroups)
{
    Console.WriteLine("Name: " + group.Name);
    Console.WriteLine("Show In Menu: " + group.ShowInMenu);
    Console.WriteLine();
}

// itereren over resource‑groepen
Console.WriteLine("Project resource group count: " + project.ResourceGroups.Count);
foreach (var group in project.ResourceGroups)
{
    Console.WriteLine("Resource group Name: " + group.Name);
    Console.WriteLine("Resource group ShowInMenu" + group.ShowInMenu);
}

var otherProject = new Project(DataDir + "Blank2010.mpp");

// verwijder de groepen van een ander project
otherProject.TaskGroups.Clear();

// kopieer groepen naar een ander project
var groups = new Group[project.TaskGroups.Count];
project.TaskGroups.CopyTo(groups, 0);

foreach (var group in groups)
{
    otherProject.TaskGroups.Add(group);
}

// voeg aangepaste taakgroep toe
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

// verwijder alle groepen
List<Group> groupsToDelete = otherProject.TaskGroups.ToList();
foreach (var group in groupsToDelete)
{
    otherProject.TaskGroups.Remove(group);
}
```

### Zie ook

* class [Group](../../group/)
* class [GroupCollection](../)
* namespace [Aspose.Tasks](../../groupcollection/)
* assembly [Aspose.Tasks](../../../)


