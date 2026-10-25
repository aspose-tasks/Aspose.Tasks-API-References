---
title: "GroupCollection.Contains"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode GroupCollection. Retourne true si l'élément spécifié est trouvé dans cette collection, sinon false"
type: docs
weight: 50
url: /fr/net/aspose.tasks/groupcollection/contains/
---
## GroupCollection.Contains method

Renvoie true si l'élément spécifié est trouvé dans cette collection ; sinon, false.

```csharp
public bool Contains(Group item)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| élément | Group | l'élément spécifié à trouver. |

### Valeur de retour

true si l'élément spécifié est trouvé dans cette collection ; sinon, false.

## Exemples

Montre comment travailler avec une collection de groupes.

```csharp
var project = new Project(DataDir + "ReadGroupDefinitionData.mpp");

// itérer sur les groupes de tâches
Console.WriteLine("Print task groups of {0} project: ", project.Get(Prj.Name));
Console.WriteLine("Task Group Count: " + project.TaskGroups.Count);
foreach (var group in project.TaskGroups)
{
    Console.WriteLine("Name: " + group.Name);
    Console.WriteLine("Show In Menu: " + group.ShowInMenu);
    Console.WriteLine();
}

// itérer sur les groupes de ressources
Console.WriteLine("Project resource group count: " + project.ResourceGroups.Count);
foreach (var group in project.ResourceGroups)
{
    Console.WriteLine("Resource group Name: " + group.Name);
    Console.WriteLine("Resource group ShowInMenu" + group.ShowInMenu);
}

var otherProject = new Project(DataDir + "Blank2010.mpp");

// effacer les groupes du autre projet
otherProject.TaskGroups.Clear();

// copier les groupes vers un autre projet
var groups = new Group[project.TaskGroups.Count];
project.TaskGroups.CopyTo(groups, 0);

foreach (var group in groups)
{
    otherProject.TaskGroups.Add(group);
}

// ajouter un groupe de tâches personnalisé
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

// supprimer tous les groupes
List<Group> groupsToDelete = otherProject.TaskGroups.ToList();
foreach (var group in groupsToDelete)
{
    otherProject.TaskGroups.Remove(group);
}
```

### Voir aussi

* class [Group](../../group/)
* class [GroupCollection](../)
* namespace [Aspose.Tasks](../../groupcollection/)
* assembly [Aspose.Tasks](../../../)


