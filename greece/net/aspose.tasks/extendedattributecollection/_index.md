---
title: "Κλάση ExtendedAttributeCollection"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.ExtendedAttributeCollection κλάση. Αναπαριστά μια συλλογή αντικειμένων ExtendedAttribute"
type: docs
weight: 530
url: /el/net/aspose.tasks/extendedattributecollection/
---
## ExtendedAttributeCollection class

Αναπαριστά μια συλλογή από αντικείμενα [`ExtendedAttribute`](../extendedattribute/).

```csharp
public class ExtendedAttributeCollection : IList<ExtendedAttribute>
```

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [Count](../../aspose.tasks/extendedattributecollection/count/) { get; } | Λαμβάνει τον αριθμό των στοιχείων που περιέχονται σε αυτή τη συλλογή. |
| [IsReadOnly](../../aspose.tasks/extendedattributecollection/isreadonly/) { get; } | Λαμβάνει μια τιμή που υποδεικνύει εάν αυτή η συλλογή είναι μόνο για ανάγνωση· διαφορετικά, false. |
| [Item](../../aspose.tasks/extendedattributecollection/item/) { get; set; } | Λαμβάνει ή ορίζει το στοιχείο στον καθορισμένο δείκτη. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| [Add](../../aspose.tasks/extendedattributecollection/add/)(ExtendedAttribute) | Προσθέτει το καθορισμένο στοιχείο σε αυτή τη συλλογή. |
| [Clear](../../aspose.tasks/extendedattributecollection/clear/)() | Αφαιρεί όλα τα στοιχεία από αυτή τη συλλογή. |
| [Contains](../../aspose.tasks/extendedattributecollection/contains/)(ExtendedAttribute) | Επιστρέφει true εάν το καθορισμένο στοιχείο βρεθεί σε αυτή τη συλλογή· διαφορετικά, false. |
| [CopyTo](../../aspose.tasks/extendedattributecollection/copyto/)(ExtendedAttribute[], int) | Αντιγράφει τα στοιχεία αυτής της συλλογής στον καθορισμένο πίνακα, ξεκινώντας από τη συγκεκριμένη θέση του πίνακα. |
| [GetEnumerator](../../aspose.tasks/extendedattributecollection/getenumerator/)() | Επιστρέφει έναν απαριθμητή για αυτή τη συλλογή. |
| [IndexOf](../../aspose.tasks/extendedattributecollection/indexof/)(ExtendedAttribute) | Καθορίζει το δείκτη του καθορισμένου στοιχείου σε αυτή τη συλλογή. |
| [Insert](../../aspose.tasks/extendedattributecollection/insert/)(int, ExtendedAttribute) | Εισάγει το καθορισμένο στοιχείο στον καθορισμένο δείκτη. |
| [Remove](../../aspose.tasks/extendedattributecollection/remove/)(ExtendedAttribute) | Αφαιρεί την πρώτη εμφάνιση ενός συγκεκριμένου αντικειμένου από αυτή τη συλλογή. |
| [RemoveAt](../../aspose.tasks/extendedattributecollection/removeat/)(int) | Αφαιρεί ένα στοιχείο στον καθορισμένο δείκτη. |

## Παραδείγματα

Δείχνει πώς να χρησιμοποιήσετε συλλογές extended attribute.

```csharp
var project = new Project(DataDir + "ReadTaskExtendedAttributes.mpp");

// Λάβετε εργασία με δείκτη μηδέν
var task = project.RootTask.Children.GetById(1);

if (!task.ExtendedAttributes.IsReadOnly && task.ExtendedAttributes.Count > 0)
{
    // καθαρίστε τα extended attributes
    task.ExtendedAttributes.Clear();
}

// δημιουργήστε ορισμό extended attribute για μια εργασία
var taskDefinition1 = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Start, ExtendedAttributeTask.Start7, "Start 7");
var taskDefinition2 = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Finish, ExtendedAttributeTask.Finish7, "Finish 7");
project.ExtendedAttributes.Add(taskDefinition1);
project.ExtendedAttributes.Add(taskDefinition2);

Console.WriteLine("Iterate over task extended attributes of " + task.Get(Tsk.Name) + " task: ");
foreach (var attribute in task.ExtendedAttributes)
{
    Console.WriteLine("Attribute FieldId: " + attribute.FieldId);
    Console.WriteLine("Attribute Value: " + attribute.DateValue);
    Console.WriteLine();
}

// Προσθέστε extended attribute 1
var extendedAttribute1 = taskDefinition1.CreateExtendedAttribute();
extendedAttribute1.DateValue = new DateTime(2020, 4, 14, 8, 0, 0);
if (task.ExtendedAttributes.IndexOf(extendedAttribute1) < 0)
{
    task.ExtendedAttributes.Insert(0, extendedAttribute1);
}

// Προσθέστε extended attribute 2
var extendedAttribute2 = taskDefinition2.CreateExtendedAttribute();
extendedAttribute2.DateValue = new DateTime(2020, 4, 14, 17, 0, 0);
task.ExtendedAttributes.Add(extendedAttribute2);

// εργαστείτε με extended attributes...

// αφαιρέστε extended attribute κατά δείκτη
task.ExtendedAttributes.RemoveAt(0);

Console.WriteLine("Count of task's extended attributes: " + task.ExtendedAttributes.Count);

// χρησιμοποιήστε πρόσβαση δείκτη συλλογής
Console.WriteLine("Attribute 1 Value: " + task.ExtendedAttributes[0].DateValue);

var otherProject = new Project();
var otherTask = otherProject.RootTask.Children.Add("Other task");

// αντιγράψτε τα attributes σε άλλο project
var attributes = new ExtendedAttribute[task.ExtendedAttributes.Count];
task.ExtendedAttributes.CopyTo(attributes, 0);

foreach (var attribute in attributes)
{
    otherTask.ExtendedAttributes.Add(attribute);
}

Console.WriteLine();
Console.WriteLine("Iterate over other task's extended attributes: ");
foreach (var attribute in otherTask.ExtendedAttributes)
{
    Console.WriteLine("Other attribute FieldId: " + attribute.FieldId);
    Console.WriteLine("Other attribute Value: " + attribute.DateValue);
    Console.WriteLine();
}

if (task.ExtendedAttributes.Contains(extendedAttribute2))
{
    task.ExtendedAttributes.Remove(extendedAttribute2);
}

// αφαιρέστε όλους τους ορισμούς extended attribute
while (otherTask.ExtendedAttributes.Count > 0)
{
    otherTask.ExtendedAttributes.Remove(otherTask.ExtendedAttributes[0]);
}
```

### Δείτε επίσης

* class [ExtendedAttribute](../extendedattribute/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


