---
title: "Classe GroupCollection"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.GroupCollection. Contient une liste d'objets Group. Implémente l'interface ICollectionGroup"
type: docs
weight: 780
url: /fr/net/aspose.tasks/groupcollection/
---
## GroupCollection class

Contient une liste d'objets [`Group`](../group/) . Implémente l'interface ICollection&lt;Group&gt;.

```csharp
public class GroupCollection : ICollection<Group>
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Count](../../aspose.tasks/groupcollection/count/) { get; } | Obtient le nombre d'éléments contenus dans cette collection. |
| [IsReadOnly](../../aspose.tasks/groupcollection/isreadonly/) { get; } | Obtient une valeur indiquant si cette collection est en lecture seule. |

## Méthodes

| Nom | Description |
| --- | --- |
| [Add](../../aspose.tasks/groupcollection/add/)(Group) | Ajoute l'élément spécifié à cette collection. |
| [Clear](../../aspose.tasks/groupcollection/clear/)() | Supprime tous les éléments de cette collection. |
| [Contains](../../aspose.tasks/groupcollection/contains/)(Group) | Renvoie true si l'élément spécifié est trouvé dans cette collection ; sinon, false. |
| [CopyTo](../../aspose.tasks/groupcollection/copyto/)(Group[], int) | Copie les éléments de cette collection dans le tableau spécifié, en commençant à l'index de tableau spécifié. |
| [GetEnumerator](../../aspose.tasks/groupcollection/getenumerator/)() | Renvoie un énumérateur pour cette collection. |
| [Remove](../../aspose.tasks/groupcollection/remove/)(Group) | Supprime la première occurrence d'un objet spécifique de cette collection. |
| [ToList](../../aspose.tasks/groupcollection/tolist/)() | Convertit une collection de groupes en une liste d'objets [`Group`](../group/). |

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

* class [Group](../group/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


