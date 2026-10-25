---
title: "Κλάση GroupCollection"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κλάση Aspose.Tasks.GroupCollection. Περιέχει μια λίστα από αντικείμενα Group. Υλοποιεί τη διεπαφή ICollectionGroup."
type: docs
weight: 780
url: /el/net/aspose.tasks/groupcollection/
---
## GroupCollection class

Περιέχει μια λίστα από αντικείμενα [`Group`](../group/). Υλοποιεί τη διεπαφή ICollection&lt;Group&gt;.

```csharp
public class GroupCollection : ICollection<Group>
```

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [Count](../../aspose.tasks/groupcollection/count/) { get; } | Λαμβάνει τον αριθμό των στοιχείων που περιέχονται σε αυτή τη συλλογή. |
| [IsReadOnly](../../aspose.tasks/groupcollection/isreadonly/) { get; } | Λαμβάνει μια τιμή που υποδεικνύει εάν αυτή η συλλογή είναι μόνο για ανάγνωση. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| [Add](../../aspose.tasks/groupcollection/add/)(Group) | Προσθέτει το καθορισμένο στοιχείο σε αυτή τη συλλογή. |
| [Clear](../../aspose.tasks/groupcollection/clear/)() | Αφαιρεί όλα τα στοιχεία από αυτή τη συλλογή. |
| [Contains](../../aspose.tasks/groupcollection/contains/)(Group) | Επιστρέφει true εάν το καθορισμένο στοιχείο βρεθεί σε αυτή τη συλλογή· διαφορετικά, false. |
| [CopyTo](../../aspose.tasks/groupcollection/copyto/)(Group[], int) | Αντιγράφει τα στοιχεία αυτής της συλλογής στον καθορισμένο πίνακα, ξεκινώντας από τη συγκεκριμένη θέση του πίνακα. |
| [GetEnumerator](../../aspose.tasks/groupcollection/getenumerator/)() | Επιστρέφει έναν απαριθμητή για αυτή τη συλλογή. |
| [Remove](../../aspose.tasks/groupcollection/remove/)(Group) | Αφαιρεί την πρώτη εμφάνιση ενός συγκεκριμένου αντικειμένου από αυτή τη συλλογή. |
| [ToList](../../aspose.tasks/groupcollection/tolist/)() | Μετατρέπει μια συλλογή ομάδων σε λίστα από αντικείμενα [`Group`](../group/). |

## Παραδείγματα

Δείχνει πώς να εργαστείτε με μια συλλογή ομάδων.

```csharp
var project = new Project(DataDir + "ReadGroupDefinitionData.mpp");

// επανάληψη στις ομάδες εργασιών
Console.WriteLine("Print task groups of {0} project: ", project.Get(Prj.Name));
Console.WriteLine("Task Group Count: " + project.TaskGroups.Count);
foreach (var group in project.TaskGroups)
{
    Console.WriteLine("Name: " + group.Name);
    Console.WriteLine("Show In Menu: " + group.ShowInMenu);
    Console.WriteLine();
}

// επανάληψη στις ομάδες πόρων
Console.WriteLine("Project resource group count: " + project.ResourceGroups.Count);
foreach (var group in project.ResourceGroups)
{
    Console.WriteLine("Resource group Name: " + group.Name);
    Console.WriteLine("Resource group ShowInMenu" + group.ShowInMenu);
}

var otherProject = new Project(DataDir + "Blank2010.mpp");

// καθαρισμός των ομάδων του άλλου έργου
otherProject.TaskGroups.Clear();

// αντιγραφή ομάδων σε άλλο έργο
var groups = new Group[project.TaskGroups.Count];
project.TaskGroups.CopyTo(groups, 0);

foreach (var group in groups)
{
    otherProject.TaskGroups.Add(group);
}

// προσθήκη προσαρμοσμένης ομάδας εργασιών
var customGroup = new Group
{
    Name = "Custom Group",
    ShowInMenu = true
};

if (!otherProject.TaskGroups.Contains(customGroup))
{
    if (!otherProject.TaskGroups.IsReadOnly)
    {
        otherProject.TaskGroups.Add(customGroup);
    }
}

// αφαίρεση όλων των ομάδων
List<Group> groupsToDelete = otherProject.TaskGroups.ToList();
foreach (var group in groupsToDelete)
{
    otherProject.TaskGroups.Remove(group);
}
```

### Δείτε επίσης

* class [Group](../group/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


