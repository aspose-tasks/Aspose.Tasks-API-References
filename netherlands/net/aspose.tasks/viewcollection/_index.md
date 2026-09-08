---
title: "Klasse ViewCollection"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.ViewCollection klasse. Bevat een lijst met View-objecten. Implementeert de ICollectionView-interface"
type: docs
weight: 2900
url: /nl/net/aspose.tasks/viewcollection/
---
## ViewCollection class

Bevat een lijst met [`View`](../view/) objecten. Implementeert de ICollection&lt;View&gt;-interface.

```csharp
public class ViewCollection : ICollection<View>
```

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [Count](../../aspose.tasks/viewcollection/count/) { get; } | Haalt het aantal elementen op dat in deze collectie zit. |
| [IsReadOnly](../../aspose.tasks/viewcollection/isreadonly/) { get; } | Haalt een waarde op die aangeeft of deze collectie alleen-lezen is; anders, false. |
| [ParentProject](../../aspose.tasks/viewcollection/parentproject/) { get; } | Haalt de bovenliggende van het View-object op. Alleen-lezen [`Project`](../project/). |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| [Add](../../aspose.tasks/viewcollection/add/)(View) | Voegt het opgegeven item toe aan deze collectie. |
| [Clear](../../aspose.tasks/viewcollection/clear/)() | Verwijdert alle items uit deze collectie. |
| [Contains](../../aspose.tasks/viewcollection/contains/)(View) | Retourneert true als het opgegeven item in deze collectie wordt gevonden; anders false. |
| [CopyTo](../../aspose.tasks/viewcollection/copyto/)(View[], int) | Kopieert de elementen van deze collectie naar de opgegeven array, beginnend bij de opgegeven array-index. |
| [GetByName](../../aspose.tasks/viewcollection/getbyname/)(string) | Zoekt naar een View met de naam en retourneert de eerste vondst binnen de collectie. |
| [GetByViewScreen](../../aspose.tasks/viewcollection/getbyviewscreen/)(ViewScreen) | Zoekt naar een View met de opgegeven Screen-eigenschap en retourneert de eerste vondst binnen de collectie. |
| [GetEnumerator](../../aspose.tasks/viewcollection/getenumerator/)() | Retourneert een enumerator voor deze collectie. |
| [Remove](../../aspose.tasks/viewcollection/remove/)(View) | Verwijdert de eerste instantie van een specifiek object uit deze collectie. |
| [ToList](../../aspose.tasks/viewcollection/tolist/)() | Converteert een view-collectie naar een lijst met [`View`](../view/) objecten. |

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

* class [View](../view/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


