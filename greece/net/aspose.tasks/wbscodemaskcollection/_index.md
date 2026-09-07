---
title: "Κλάση WBSCodeMaskCollection"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κλάση Aspose.Tasks.WBSCodeMaskCollection. Αντιπροσωπεύει μια συλλογή αντικειμένων WBSCodeMask"
type: docs
weight: 3510
url: /el/net/aspose.tasks/wbscodemaskcollection/
---
## WBSCodeMaskCollection class

Αντιπροσωπεύει μια συλλογή από αντικείμενα WBSCodeMask.

```csharp
public class WBSCodeMaskCollection : IList<WBSCodeMask>
```

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [Count](../../aspose.tasks/wbscodemaskcollection/count/) { get; } | Λαμβάνει τον αριθμό των στοιχείων που περιέχονται σε αυτή τη συλλογή. |
| [IsReadOnly](../../aspose.tasks/wbscodemaskcollection/isreadonly/) { get; } | Λαμβάνει μια τιμή που υποδεικνύει εάν αυτή η συλλογή είναι μόνο για ανάγνωση· διαφορετικά, false. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| [Add](../../aspose.tasks/wbscodemaskcollection/add/)(WBSCodeMask) | Προσθέτει το καθορισμένο στοιχείο σε αυτή τη συλλογή. |
| [Clear](../../aspose.tasks/wbscodemaskcollection/clear/)() | Αφαιρεί όλα τα στοιχεία από αυτή τη συλλογή. |
| [Contains](../../aspose.tasks/wbscodemaskcollection/contains/)(WBSCodeMask) | Επιστρέφει true εάν το καθορισμένο στοιχείο βρεθεί σε αυτή τη συλλογή· διαφορετικά, false. |
| [CopyTo](../../aspose.tasks/wbscodemaskcollection/copyto/)(WBSCodeMask[], int) | Αντιγράφει τα στοιχεία αυτής της συλλογής στον καθορισμένο πίνακα, ξεκινώντας από τη συγκεκριμένη θέση του πίνακα. |
| [GetEnumerator](../../aspose.tasks/wbscodemaskcollection/getenumerator/)() | Επιστρέφει έναν απαριθμητή για αυτή τη συλλογή. |
| [Remove](../../aspose.tasks/wbscodemaskcollection/remove/)(WBSCodeMask) | Αφαιρεί την πρώτη εμφάνιση ενός συγκεκριμένου αντικειμένου από αυτή τη συλλογή. |
| [ToList](../../aspose.tasks/wbscodemaskcollection/tolist/)() | Μετατρέπει μια WBSCodeMaskCollection σε λίστα αντικειμένων [`WBSCodeMask`](../wbscodemask/). |

## Παραδείγματα

Δείχνει πώς να εργαστείτε με τη συλλογή WBS code mask.

```csharp
var project = new Project();

project.WBSCodeDefinition = new WBSCodeDefinition();
project.WBSCodeDefinition.GenerateWBSCode = true;
project.WBSCodeDefinition.VerifyUniqueness = true;
project.WBSCodeDefinition.CodePrefix = "CRS-";

project.WBSCodeDefinition.CodeMaskCollection.Clear();

var mask1 = new WBSCodeMask();
mask1.Length = 2;
mask1.Separator = "-";
mask1.Sequence = WBSSequence.OrderedNumbers;
project.WBSCodeDefinition.CodeMaskCollection.Add(mask1);

var mask2 = new WBSCodeMask();
mask2.Length = 1;
mask2.Separator = "-";
mask2.Sequence = WBSSequence.OrderedUppercaseLetters;
project.WBSCodeDefinition.CodeMaskCollection.Add(mask2);

Console.WriteLine("WBS Code mask's count: " + project.WBSCodeDefinition.CodeMaskCollection.Count);
Console.WriteLine("Is WBS Code mask collection read-only?: " + project.WBSCodeDefinition.CodeMaskCollection.IsReadOnly);
Console.WriteLine("Masks: ");
Console.WriteLine();
foreach (var wbsMask in project.WBSCodeDefinition.CodeMaskCollection)
{
    Console.WriteLine("Length: " + wbsMask.Length);
    Console.WriteLine("Level: " + wbsMask.Level);
    Console.WriteLine("Separator: " + wbsMask.Separator);
    Console.WriteLine("Sequence: " + wbsMask.Sequence);
    Console.WriteLine();
}

var task1 = project.RootTask.Children.Add("Task 1");
task1.Children.Add("Task 2");

project.Recalculate();

IEnumerable<Task> childTasks = project.RootTask.SelectAllChildTasks();
foreach (var childTask in childTasks)
{
    Console.WriteLine("Task name: " + childTask.Get(Tsk.Name));
    Console.WriteLine("Task WBS code: " + childTask.Get(Tsk.WBS));
}

project.WBSCodeDefinition.CodeMaskCollection.Remove(mask2);

if (project.WBSCodeDefinition.CodeMaskCollection.Contains(mask2))
{
    throw new InvalidOperationException("WBS code mask wasn't removed.");
}

var otherProject = new Project();
otherProject.WBSCodeDefinition = new WBSCodeDefinition();
otherProject.WBSCodeDefinition.GenerateWBSCode = true;
otherProject.WBSCodeDefinition.VerifyUniqueness = true;
otherProject.WBSCodeDefinition.CodePrefix = "CRS-";

// αντιγράψτε τις μάσκες κώδικα σε άλλο έργο
var masks = new WBSCodeMask[project.WBSCodeDefinition.CodeMaskCollection.Count];
project.WBSCodeDefinition.CodeMaskCollection.CopyTo(masks, 0);

foreach (var mask in masks)
{
    otherProject.WBSCodeDefinition.CodeMaskCollection.Add(mask);
}

List<WBSCodeMask> wbsMasks = otherProject.WBSCodeDefinition.CodeMaskCollection.ToList();
foreach (var wbsMask in wbsMasks)
{
    Console.WriteLine("Length: " + wbsMask.Length);
    Console.WriteLine("Level: " + wbsMask.Level);
    Console.WriteLine("Separator: " + wbsMask.Separator);
    Console.WriteLine("Sequence: " + wbsMask.Sequence);
    Console.WriteLine();
}

var otherTask1 = project.RootTask.Children.Add("Other task 1");
otherTask1.Children.Add("Other task 2");

otherProject.Recalculate();

Console.WriteLine("Print WBS codes of the other project: ");
IEnumerable<Task> otherChildTasks = otherProject.RootTask.SelectAllChildTasks();
foreach (var childTask in otherChildTasks)
{
    Console.WriteLine("Task name: " + childTask.Get(Tsk.Name));
    Console.WriteLine("Task WBS code: " + childTask.Get(Tsk.WBS));
}
```

### Δείτε επίσης

* class [WBSCodeMask](../wbscodemask/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


