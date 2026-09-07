---
title: "Κλάση ViewCollection"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Η κλάση Aspose.Tasks.ViewCollection. Περιέχει μια λίστα αντικειμένων View. Υλοποιεί τη διεπαφή ICollectionView"
type: docs
weight: 2900
url: /el/net/aspose.tasks/viewcollection/
---
## ViewCollection class

Περιέχει μια λίστα αντικειμένων [`View`](../view/). Υλοποιεί τη διεπαφή ICollection&lt;View&gt;.

```csharp
public class ViewCollection : ICollection<View>
```

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [Count](../../aspose.tasks/viewcollection/count/) { get; } | Λαμβάνει τον αριθμό των στοιχείων που περιέχονται σε αυτή τη συλλογή. |
| [IsReadOnly](../../aspose.tasks/viewcollection/isreadonly/) { get; } | Λαμβάνει μια τιμή που υποδεικνύει εάν αυτή η συλλογή είναι μόνο για ανάγνωση· διαφορετικά, false. |
| [ParentProject](../../aspose.tasks/viewcollection/parentproject/) { get; } | Λαμβάνει το γονέα του αντικειμένου View. Μόνο για ανάγνωση [`Project`](../project/). |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| [Add](../../aspose.tasks/viewcollection/add/)(View) | Προσθέτει το καθορισμένο στοιχείο σε αυτή τη συλλογή. |
| [Clear](../../aspose.tasks/viewcollection/clear/)() | Αφαιρεί όλα τα στοιχεία από αυτή τη συλλογή. |
| [Contains](../../aspose.tasks/viewcollection/contains/)(View) | Επιστρέφει true εάν το καθορισμένο στοιχείο βρεθεί σε αυτή τη συλλογή· διαφορετικά, false. |
| [CopyTo](../../aspose.tasks/viewcollection/copyto/)(View[], int) | Αντιγράφει τα στοιχεία αυτής της συλλογής στον καθορισμένο πίνακα, ξεκινώντας από τη συγκεκριμένη θέση του πίνακα. |
| [GetByName](../../aspose.tasks/viewcollection/getbyname/)(string) | Αναζητά ένα View με το όνομα και επιστρέφει την πρώτη εμφάνιση μέσα στη συλλογή. |
| [GetByViewScreen](../../aspose.tasks/viewcollection/getbyviewscreen/)(ViewScreen) | Αναζητά ένα View με το καθορισμένο χαρακτηριστικό Screen και επιστρέφει την πρώτη εμφάνιση μέσα στη συλλογή. |
| [GetEnumerator](../../aspose.tasks/viewcollection/getenumerator/)() | Επιστρέφει έναν απαριθμητή για αυτή τη συλλογή. |
| [Remove](../../aspose.tasks/viewcollection/remove/)(View) | Αφαιρεί την πρώτη εμφάνιση ενός συγκεκριμένου αντικειμένου από αυτή τη συλλογή. |
| [ToList](../../aspose.tasks/viewcollection/tolist/)() | Μετατρέπει μια συλλογή προβολών σε λίστα αντικειμένων [`View`](../view/). |

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

* class [View](../view/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


