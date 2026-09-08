---
title: "ViewCollection.Contains"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "ViewCollection method. Retourneert true als het opgegeven item in deze collectie wordt gevonden, anders false"
type: docs
weight: 60
url: /nl/net/aspose.tasks/viewcollection/contains/
---
## ViewCollection.Contains method

Retourneert true als het opgegeven item in deze collectie wordt gevonden; anders false.

```csharp
public bool Contains(View item)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| item | View | het opgegeven item om te vinden. |

### Retourwaarde

true als het opgegeven item in deze collectie wordt gevonden; anders false.

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

* class [View](../../view/)
* class [ViewCollection](../)
* namespace [Aspose.Tasks](../../viewcollection/)
* assembly [Aspose.Tasks](../../../)


