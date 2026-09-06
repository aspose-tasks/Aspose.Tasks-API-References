---
title: "ViewCollection.ToList"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "ViewCollection méthode. Convertit une collection de vues en une liste d'objets View"
type: docs
weight: 120
url: /fr/net/aspose.tasks/viewcollection/tolist/
---
## ViewCollection.ToList method

Convertit une collection de vues en une liste d'objets [`View`](../../view/).

```csharp
public List<View> ToList()
```

### Valeur de retour

Liste générique d'objets [`View`](../../view/).

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

* class [View](../../view/)
* class [ViewCollection](../)
* namespace [Aspose.Tasks](../../viewcollection/)
* assembly [Aspose.Tasks](../../../)


