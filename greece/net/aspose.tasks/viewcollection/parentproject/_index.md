---
title: "ViewCollection.ParentProject"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα ViewCollection. Λαμβάνει το γονικό αντικείμενο της κλάσης View. Έργο μόνο για ανάγνωση"
type: docs
weight: 30
url: /el/net/aspose.tasks/viewcollection/parentproject/
---
## ViewCollection.ParentProject property

Λαμβάνει το γονικό αντικείμενο του View. Μόνο ανάγνωση [`Project`](../../project/).

```csharp
public Project ParentProject { get; }
```

## Παραδείγματα

Δείχνει πώς να εργαστείτε με συλλογές προβολών.

```csharp
var project = new Project(DataDir + "Project1.mpp");

// μετατροπή σε απλή λίστα προβολών
List<View> list = project.Views.ToList();
for (var index = 0; index < list.Count; index++)
{
    var viewToChange = list[index];
    viewToChange.PageInfo.Header.CenteredText = "Header " + index;
}

// προσθήκη νέας προβολής
var view = new GanttChartView();
if (!project.Views.IsReadOnly)
{
    project.Views.Add(view);
}

// επανάληψη στις προβολές
Console.WriteLine("Iterate over views of " + project.Views.ParentProject.Get(Prj.Name) + " project.");
Console.WriteLine("Project view count: " + project.Views.Count);
Console.WriteLine();
foreach (var projectView in project.Views)
{
    Console.WriteLine("Name: " + projectView.Name);
}

// αφαίρεση όλων των προβολών ταυτόχρονα
project.Views.Clear();

// ή μία-μία
{
    // πρόσβαση 1
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
    // πρόσβαση 2
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

### Δείτε επίσης

* class [Project](../../project/)
* class [ViewCollection](../)
* namespace [Aspose.Tasks](../../viewcollection/)
* assembly [Aspose.Tasks](../../../)


