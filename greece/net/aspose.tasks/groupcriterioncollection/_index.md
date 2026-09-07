---
title: "Κλάση GroupCriterionCollection"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Η κλάση Aspose.Tasks.GroupCriterionCollection. Περιέχει μια συλλογή αντικειμένων GroupCriterion. Υλοποιεί τη διεπαφή ICollectionGroupCriterion."
type: docs
weight: 800
url: /el/net/aspose.tasks/groupcriterioncollection/
---
## GroupCriterionCollection class

Περιέχει μια συλλογή από αντικείμενα [`GroupCriterion`](../groupcriterion/). Υλοποιεί τη διεπαφή ICollection&lt;GroupCriterion&gt;.

```csharp
public class GroupCriterionCollection : IList<GroupCriterion>
```

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [Count](../../aspose.tasks/groupcriterioncollection/count/) { get; } | Λαμβάνει τον αριθμό των στοιχείων που περιέχονται σε αυτή τη συλλογή. |
| [IsReadOnly](../../aspose.tasks/groupcriterioncollection/isreadonly/) { get; } | Λαμβάνει μια τιμή που υποδεικνύει εάν αυτή η συλλογή είναι μόνο για ανάγνωση· διαφορετικά, false. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| [Add](../../aspose.tasks/groupcriterioncollection/add/)(GroupCriterion) | Προσθέτει το καθορισμένο στοιχείο σε αυτή τη συλλογή. |
| [Clear](../../aspose.tasks/groupcriterioncollection/clear/)() | Αφαιρεί όλα τα στοιχεία από αυτή τη συλλογή. |
| [Contains](../../aspose.tasks/groupcriterioncollection/contains/)(GroupCriterion) | Επιστρέφει true εάν το καθορισμένο στοιχείο βρεθεί σε αυτή τη συλλογή· διαφορετικά, false. |
| [CopyTo](../../aspose.tasks/groupcriterioncollection/copyto/)(GroupCriterion[], int) | Αντιγράφει τα στοιχεία αυτής της συλλογής στον καθορισμένο πίνακα, ξεκινώντας από τη συγκεκριμένη θέση του πίνακα. |
| [GetEnumerator](../../aspose.tasks/groupcriterioncollection/getenumerator/)() | Επιστρέφει έναν απαριθμητή για αυτή τη συλλογή. |
| [Remove](../../aspose.tasks/groupcriterioncollection/remove/)(GroupCriterion) | Αφαιρεί την πρώτη εμφάνιση ενός συγκεκριμένου αντικειμένου από αυτή τη συλλογή. |
| [ToList](../../aspose.tasks/groupcriterioncollection/tolist/)() | Μετατρέπει μια συλλογή GroupCriterion σε λίστα από αντικείμενα [`GroupCriterion`](../groupcriterion/). |

## Παραδείγματα

Δείχνει πώς να εργαστείτε με μια συλλογή κριτηρίων ομάδας.

```csharp
var project = new Project(DataDir + "ReadGroupDefinitionData.mpp");

var group = project.TaskGroups.ToList()[0];

// επανάληψη πάνω από κριτήρια ομάδας
Console.WriteLine("Print group criteria of the group '{0}': ", group.Name);
Console.WriteLine("Group criterion count: " + group.GroupCriteria.Count);
foreach (var criterion in group.GroupCriteria)
{
    Console.WriteLine("Field: " + criterion.Field);
    Console.WriteLine("Group On: " + criterion.GroupOn);
    Console.WriteLine();
}

group.GroupCriteria.Clear();

if (!group.GroupCriteria.IsReadOnly)
{
    List<GroupCriterion> groupCriteria = group.GroupCriteria.ToList();
    foreach (var criterion in groupCriteria)
    {
        group.GroupCriteria.Remove(criterion);
    }
}

var criterionToAdd = new GroupCriterion
{
    Ascending = true,
    Field = Field.TaskActive
};

if (!group.GroupCriteria.Contains(criterionToAdd))
{
    group.GroupCriteria.Add(criterionToAdd);
}

// αντιγραφή κριτηρίων σε άλλη ομάδα
var otherGroup = project.TaskGroups.ToList()[0];

var criteria = new GroupCriterion[group.GroupCriteria.Count];
group.GroupCriteria.CopyTo(criteria, 0);
foreach (var criterion in criteria)
{
    otherGroup.GroupCriteria.Add(criterion);
}
```

### Δείτε επίσης

* class [GroupCriterion](../groupcriterion/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


