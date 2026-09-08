---
title: "ViewCollection.Count"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "ViewCollection property. Geeft het aantal elementen terug dat in deze collectie zit"
type: docs
weight: 10
url: /nl/net/aspose.tasks/viewcollection/count/
---
## ViewCollection.Count property

Haalt het aantal elementen op dat in deze collectie zit.

```csharp
public int Count { get; }
```

## Voorbeelden

Toont hoe te werken met view-collecties.

```csharp
var project = new Project(DataDir + "Project1.mpp");

// converteer naar een eenvoudige lijst met views
List<View> list = project.Views.ToList();
for (var index = 0; index < list.Count; index++)
{
    var viewToChange = list[index];
    viewToChange.PageInfo.Header.CenteredText = "Header " + index;
}

// voeg een nieuwe view toe
var view = new GanttChartView();
if (!project.Views.IsReadOnly)
{
    project.Views.Add(view);
}

// itereren over views
Console.WriteLine("Iterate over views of " + project.Views.ParentProject.Get(Prj.Name) + " project.");
Console.WriteLine("Project view count: " + project.Views.Count);
Console.WriteLine();
foreach (var projectView in project.Views)
{
    Console.WriteLine("Name: " + projectView.Name);
}

// verwijder alle views in één keer
project.Views.Clear();

// of één voor één
{
    // aanpak 1
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
    // aanpak 2
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

### Zie ook

* class [ViewCollection](../)
* namespace [Aspose.Tasks](../../viewcollection/)
* assembly [Aspose.Tasks](../../../)


