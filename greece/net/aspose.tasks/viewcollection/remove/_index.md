---
title: "ViewCollection.Remove"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος ViewCollection. Αφαιρεί την πρώτη εμφάνιση ενός συγκεκριμένου αντικειμένου από αυτή τη συλλογή"
type: docs
weight: 110
url: /el/net/aspose.tasks/viewcollection/remove/
---
## ViewCollection.Remove method

Αφαιρεί την πρώτη εμφάνιση ενός συγκεκριμένου αντικειμένου από αυτή τη συλλογή.

```csharp
public bool Remove(View item)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| item | View | το καθορισμένο αντικείμενο προς αφαίρεση. |

### Τιμή Επιστροφής

αληθές εάν το καθορισμένο αντικείμενο αφαιρέθηκε επιτυχώς από αυτή τη συλλογή· διαφορετικά, ψευδές.

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

* class [View](../../view/)
* class [ViewCollection](../)
* namespace [Aspose.Tasks](../../viewcollection/)
* assembly [Aspose.Tasks](../../../)


