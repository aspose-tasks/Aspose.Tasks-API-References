---
title: "Classe ViewCollection"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.ViewCollection. Contient une liste d'objets View. Implémente l'interface ICollectionView"
type: docs
weight: 2900
url: /fr/net/aspose.tasks/viewcollection/
---
## ViewCollection class

Contient une liste d'objets [`View`](../view/). Implémente l'interface ICollection&lt;View&gt;.

```csharp
public class ViewCollection : ICollection<View>
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Count](../../aspose.tasks/viewcollection/count/) { get; } | Obtient le nombre d'éléments contenus dans cette collection. |
| [IsReadOnly](../../aspose.tasks/viewcollection/isreadonly/) { get; } | Obtient une valeur indiquant si cette collection est en lecture seule ; sinon, false. |
| [ParentProject](../../aspose.tasks/viewcollection/parentproject/) { get; } | Obtient le parent de l’objet View. Lecture seule [`Project`](../project/). |

## Méthodes

| Nom | Description |
| --- | --- |
| [Add](../../aspose.tasks/viewcollection/add/)(View) | Ajoute l'élément spécifié à cette collection. |
| [Clear](../../aspose.tasks/viewcollection/clear/)() | Supprime tous les éléments de cette collection. |
| [Contains](../../aspose.tasks/viewcollection/contains/)(View) | Renvoie true si l'élément spécifié est trouvé dans cette collection ; sinon, false. |
| [CopyTo](../../aspose.tasks/viewcollection/copyto/)(View[], int) | Copie les éléments de cette collection dans le tableau spécifié, en commençant à l'index de tableau spécifié. |
| [GetByName](../../aspose.tasks/viewcollection/getbyname/)(string) | Recherche une View avec le nom et renvoie la première occurrence dans la collection. |
| [GetByViewScreen](../../aspose.tasks/viewcollection/getbyviewscreen/)(ViewScreen) | Recherche une View avec la propriété Screen spécifiée et renvoie la première occurrence dans la collection. |
| [GetEnumerator](../../aspose.tasks/viewcollection/getenumerator/)() | Renvoie un énumérateur pour cette collection. |
| [Remove](../../aspose.tasks/viewcollection/remove/)(View) | Supprime la première occurrence d'un objet spécifique de cette collection. |
| [ToList](../../aspose.tasks/viewcollection/tolist/)() | Convertit une collection de vues en une liste d'objets [`View`](../view/). |

## Exemples

Montre comment travailler avec des collections de vues.

```csharp
var project = new Project(DataDir + "Project1.mpp");

// convertir en une liste simple de vues
List<View> list = project.Views.ToList();
for (var index = 0; index < list.Count; index++)
{
    var viewToChange = list[index];
    viewToChange.PageInfo.Header.CenteredText = "Header " + index;
}

// ajouter une nouvelle vue
var view = new GanttChartView();
if (!project.Views.IsReadOnly)
{
    project.Views.Add(view);
}

// itérer sur les vues
Console.WriteLine("Iterate over views of " + project.Views.ParentProject.Get(Prj.Name) + " project.");
Console.WriteLine("Project view count: " + project.Views.Count);
Console.WriteLine();
foreach (var projectView in project.Views)
{
    Console.WriteLine("Name: " + projectView.Name);
}

// supprimer toutes les vues d'un coup
project.Views.Clear();

// ou une par une
{
    // approche 1
    List<View> listToDelete = project.Views.ToList();
    foreach (var v in listToDelete)
    {
        if (project.Views.Contains(v))
        {
            project.Views.Remove(v);
        }
    }
}

{
    // approche 2
    var array = new View[project.Views.Count];
    project.Views.CopyTo(array, 0);
    foreach (var v in array)
    {
        if (project.Views.Contains(v))
        {
            project.Views.Remove(v);
        }
    }
}
```

### Voir aussi

* class [View](../view/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


