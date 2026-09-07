---
title: "ViewCollection.ToList"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "ViewCollection metodo. Converte una collezione di visualizzazioni in un elenco di oggetti View"
type: docs
weight: 120
url: /it/net/aspose.tasks/viewcollection/tolist/
---
## ViewCollection.ToList method

Converte una collezione di visualizzazioni in un elenco di oggetti [`View`](../../view/).

```csharp
public List<View> ToList()
```

### Valore di ritorno

Elenco generico di oggetti [`View`](../../view/).

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

* class [View](../../view/)
* class [ViewCollection](../)
* namespace [Aspose.Tasks](../../viewcollection/)
* assembly [Aspose.Tasks](../../../)


