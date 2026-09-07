---
title: "ViewCollection.Count"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "ViewCollection proprietà. Ottiene il numero di elementi contenuti in questa collezione"
type: docs
weight: 10
url: /it/net/aspose.tasks/viewcollection/count/
---
## ViewCollection.Count property

Ottiene il numero di elementi contenuti in questa collezione.

```csharp
public int Count { get; }
```

## Esempi

Mostra come lavorare con le collezioni di view.

```csharp
var project = new Project(DataDir + "Project1.mpp");

// converti in un semplice elenco di view
List<View> list = project.Views.ToList();
for (var index = 0; index < list.Count; index++)
{
    var viewToChange = list[index];
    viewToChange.PageInfo.Header.CenteredText = "Header " + index;
}

// aggiungi una nuova view
var view = new GanttChartView();
if (!project.Views.IsReadOnly)
{
    project.Views.Add(view);
}

// itera sulle view
Console.WriteLine("Iterate over views of " + project.Views.ParentProject.Get(Prj.Name) + " project.");
Console.WriteLine("Project view count: " + project.Views.Count);
Console.WriteLine();
foreach (var projectView in project.Views)
{
    Console.WriteLine("Name: " + projectView.Name);
}

// rimuovi tutte le view in una volta
project.Views.Clear();

// oppure una alla volta
{
    // approccio 1
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
    // approccio 2
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

### Vedi anche

* class [ViewCollection](../)
* namespace [Aspose.Tasks](../../viewcollection/)
* assembly [Aspose.Tasks](../../../)


