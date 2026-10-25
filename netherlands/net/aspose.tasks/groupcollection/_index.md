---
title: "Klasse GroupCollection"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.GroupCollection klasse. Bevat een lijst van Group‑objecten. Implementeert de ICollectionGroup‑interface."
type: docs
weight: 780
url: /nl/net/aspose.tasks/groupcollection/
---
## GroupCollection class

Bevat een lijst van [`Group`](../group/) objecten. Implementeert de ICollection&lt;Group&gt; interface.

```csharp
public class GroupCollection : ICollection<Group>
```

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [Count](../../aspose.tasks/groupcollection/count/) { get; } | Haalt het aantal elementen op dat in deze collectie zit. |
| [IsReadOnly](../../aspose.tasks/groupcollection/isreadonly/) { get; } | Haalt een waarde op die aangeeft of deze collectie alleen-lezen is. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| [Add](../../aspose.tasks/groupcollection/add/)(Group) | Voegt het opgegeven item toe aan deze collectie. |
| [Clear](../../aspose.tasks/groupcollection/clear/)() | Verwijdert alle items uit deze collectie. |
| [Contains](../../aspose.tasks/groupcollection/contains/)(Group) | Retourneert true als het opgegeven item in deze collectie wordt gevonden; anders false. |
| [CopyTo](../../aspose.tasks/groupcollection/copyto/)(Group[], int) | Kopieert de elementen van deze collectie naar de opgegeven array, beginnend bij de opgegeven array-index. |
| [GetEnumerator](../../aspose.tasks/groupcollection/getenumerator/)() | Retourneert een enumerator voor deze collectie. |
| [Remove](../../aspose.tasks/groupcollection/remove/)(Group) | Verwijdert de eerste instantie van een specifiek object uit deze collectie. |
| [ToList](../../aspose.tasks/groupcollection/tolist/)() | Converteert een groepscollectie naar een lijst van [`Group`](../group/) objecten. |

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

* class [Group](../group/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


