---
title: "Κλάση ExtendedAttributeDefinitionCollection"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κλάση Aspose.Tasks.ExtendedAttributeDefinitionCollection. Αντιπροσωπεύει μια συλλογή αντικειμένων ExtendedAttributeDefinition"
type: docs
weight: 550
url: /el/net/aspose.tasks/extendedattributedefinitioncollection/
---
## ExtendedAttributeDefinitionCollection class

Αντιπροσωπεύει μια συλλογή αντικειμένων [`ExtendedAttributeDefinition`](../extendedattributedefinition/).

```csharp
public class ExtendedAttributeDefinitionCollection : IList<ExtendedAttributeDefinition>
```

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [Count](../../aspose.tasks/extendedattributedefinitioncollection/count/) { get; } | Λαμβάνει τον αριθμό των στοιχείων που περιέχονται σε αυτή τη συλλογή. |
| [IsReadOnly](../../aspose.tasks/extendedattributedefinitioncollection/isreadonly/) { get; } | Λαμβάνει μια τιμή που υποδεικνύει εάν αυτή η συλλογή είναι μόνο για ανάγνωση. |
| [Item](../../aspose.tasks/extendedattributedefinitioncollection/item/) { get; set; } | Επιστρέφει ή ορίζει το στοιχείο στη συγκεκριμένη θέση. |
| [ParentProject](../../aspose.tasks/extendedattributedefinitioncollection/parentproject/) { get; } | Λαμβάνει ένα γονικό έργο για την παρουσία `ExtendedAttributeDefinitionCollection`. Επιστρέφει ένα γονικό έργο για αυτή τη συλλογή. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| [Add](../../aspose.tasks/extendedattributedefinitioncollection/add/)(ExtendedAttributeDefinition) | Προσθέτει το καθορισμένο στοιχείο σε αυτή τη συλλογή. |
| [Clear](../../aspose.tasks/extendedattributedefinitioncollection/clear/)() | Αφαιρεί όλα τα στοιχεία από αυτή τη συλλογή. |
| [Contains](../../aspose.tasks/extendedattributedefinitioncollection/contains/)(ExtendedAttributeDefinition) | Επιστρέφει true εάν το καθορισμένο στοιχείο βρεθεί σε αυτή τη συλλογή· διαφορετικά, false. |
| [CopyTo](../../aspose.tasks/extendedattributedefinitioncollection/copyto/)(ExtendedAttributeDefinition[], int) | Αντιγράφει τα στοιχεία αυτής της συλλογής στον καθορισμένο πίνακα, ξεκινώντας από τη συγκεκριμένη θέση του πίνακα. |
| [GetById](../../aspose.tasks/extendedattributedefinitioncollection/getbyid/)(int) | Επιστρέφει έναν ορισμό εκτεταμένου χαρακτηριστικού με βάση το αναγνωριστικό |
| [GetEnumerator](../../aspose.tasks/extendedattributedefinitioncollection/getenumerator/)() | Επιστρέφει έναν απαριθμητή για αυτή τη συλλογή. |
| [IndexOf](../../aspose.tasks/extendedattributedefinitioncollection/indexof/)(ExtendedAttributeDefinition) | Καθορίζει το δείκτη του καθορισμένου στοιχείου σε αυτή τη συλλογή. |
| [Insert](../../aspose.tasks/extendedattributedefinitioncollection/insert/)(int, ExtendedAttributeDefinition) | Εισάγει το καθορισμένο στοιχείο στον καθορισμένο δείκτη. |
| [Remove](../../aspose.tasks/extendedattributedefinitioncollection/remove/)(ExtendedAttributeDefinition) | Αφαιρεί την πρώτη εμφάνιση ενός συγκεκριμένου αντικειμένου από αυτή τη συλλογή. |
| [RemoveAt](../../aspose.tasks/extendedattributedefinitioncollection/removeat/)(int) | Αφαιρεί ένα στοιχείο στον καθορισμένο δείκτη. |
| [ToList](../../aspose.tasks/extendedattributedefinitioncollection/tolist/)() | Μετατρέπει αυτό το αντικείμενο ExtendedAttributeDefinitionCollection σε λίστα που περιέχει παρουσίες της κλάσης [`ExtendedAttributeDefinition`](../extendedattributedefinition/). |

## Παραδείγματα

Δείχνει πώς να χρησιμοποιήσετε συλλογές ορισμών εκτεταμένων χαρακτηριστικών.

```csharp
var project = new Project(DataDir + "ReadTaskExtendedAttributes.mpp");

if (!project.ExtendedAttributes.IsReadOnly)
{
    if (project.ExtendedAttributes.Count > 0)
    {
        // καθαρισμός εκτεταμένων ορισμών χαρακτηριστικών
        project.ExtendedAttributes.Clear();
    }
}

// δημιουργήστε ορισμό extended attribute για μια εργασία
var taskDefinition = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Start, ExtendedAttributeTask.Start7, "Start 7");
project.ExtendedAttributes.Add(taskDefinition);

Console.WriteLine("Iterate over extended attributes of " + project.ExtendedAttributes.ParentProject.Get(Prj.Name) + " project: ");
foreach (var attribute in project.ExtendedAttributes)
{
    Console.WriteLine("Attribute Alias: " + attribute.Alias);
    Console.WriteLine("Attribute CfType: " + attribute.CfType);
    Console.WriteLine();
}

Console.WriteLine();

// εργασία με εκτεταμένους ορισμούς χαρακτηριστικών...
var resourceDefinition = ExtendedAttributeDefinition.CreateResourceDefinition(CustomFieldType.Cost, ExtendedAttributeResource.Cost5, "My cost");

if (!project.ExtendedAttributes.Contains(resourceDefinition))
{
    project.ExtendedAttributes.Add(resourceDefinition);
}

// εργασία με εκτεταμένους ορισμούς χαρακτηριστικών...
var resourceDefinition2 = ExtendedAttributeDefinition.CreateResourceDefinition(CustomFieldType.Number, ExtendedAttributeResource.Cost1, "My Cost 2");

if (project.ExtendedAttributes.IndexOf(resourceDefinition2) < 0)
{
    project.ExtendedAttributes.Insert(0, resourceDefinition2);
}

// εργασία με εκτεταμένους ορισμούς χαρακτηριστικών...

// αφαιρέστε extended attribute κατά δείκτη
project.ExtendedAttributes.RemoveAt(0);

Console.WriteLine("Print project's extended attributes: ");
Console.WriteLine("Count of project's extended attribute definitions: " + project.ExtendedAttributes.Count);

// χρησιμοποιήστε πρόσβαση δείκτη συλλογής
Console.WriteLine("Attribute 1 Alias: " + project.ExtendedAttributes[0].Alias);
Console.WriteLine("Attribute 1 CfType: " + project.ExtendedAttributes[0].CfType);
Console.WriteLine("Attribute 2 Alias: " + project.ExtendedAttributes[1].Alias);
Console.WriteLine("Attribute 2 CfType: " + project.ExtendedAttributes[1].CfType);

var otherProject = new Project();

// αντιγράψτε τα attributes σε άλλο project
var attributes = new ExtendedAttributeDefinition[project.ExtendedAttributes.Count];
project.ExtendedAttributes.CopyTo(attributes, 0);

foreach (var attribute in attributes)
{
    otherProject.ExtendedAttributes.Add(attribute);
}

Console.WriteLine();
Console.WriteLine("Iterate over other project's extended attributes: ");
foreach (var attribute in otherProject.ExtendedAttributes)
{
    Console.WriteLine("Attribute Alias: " + attribute.Alias);
    Console.WriteLine("Attribute CfType: " + attribute.CfType);
    Console.WriteLine();
}

// αφαιρέστε όλους τους ορισμούς extended attribute
List<ExtendedAttributeDefinition> definitions = project.ExtendedAttributes.ToList();
foreach (var definition in definitions)
{
    project.ExtendedAttributes.Remove(definition);
}
```

### Δείτε επίσης

* class [ExtendedAttributeDefinition](../extendedattributedefinition/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


