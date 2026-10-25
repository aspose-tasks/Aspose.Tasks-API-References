---
title: "Κλάση OutlineCodeDefinitionCollection"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κλάση Aspose.Tasks.OutlineCodeDefinitionCollection. Αντιπροσωπεύει μια συλλογή αντικειμένων OutlineCodeDefinition."
type: docs
weight: 1180
url: /el/net/aspose.tasks/outlinecodedefinitioncollection/
---
## OutlineCodeDefinitionCollection class

Αντιπροσωπεύει μια συλλογή αντικειμένων [`OutlineCodeDefinition`](../outlinecodedefinition/).

```csharp
public class OutlineCodeDefinitionCollection : IList<OutlineCodeDefinition>
```

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [Count](../../aspose.tasks/outlinecodedefinitioncollection/count/) { get; } | Λαμβάνει τον αριθμό των στοιχείων που περιέχονται σε αυτή τη συλλογή. |
| [IsReadOnly](../../aspose.tasks/outlinecodedefinitioncollection/isreadonly/) { get; } | Λαμβάνει μια τιμή που υποδεικνύει εάν αυτή η συλλογή είναι μόνο για ανάγνωση· διαφορετικά, false. |
| [Item](../../aspose.tasks/outlinecodedefinitioncollection/item/) { get; set; } | Επιστρέφει ή ορίζει το στοιχείο στη συγκεκριμένη θέση. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| [Add](../../aspose.tasks/outlinecodedefinitioncollection/add/)(OutlineCodeDefinition) | Προσθέτει το καθορισμένο στοιχείο σε αυτή τη συλλογή. |
| [Clear](../../aspose.tasks/outlinecodedefinitioncollection/clear/)() | Αφαιρεί όλα τα στοιχεία από αυτή τη συλλογή. |
| [Contains](../../aspose.tasks/outlinecodedefinitioncollection/contains/)(OutlineCodeDefinition) | Επιστρέφει true εάν το καθορισμένο στοιχείο βρεθεί σε αυτή τη συλλογή· διαφορετικά, false. |
| [CopyTo](../../aspose.tasks/outlinecodedefinitioncollection/copyto/)(OutlineCodeDefinition[], int) | Αντιγράφει τα στοιχεία αυτής της συλλογής στον καθορισμένο πίνακα, ξεκινώντας από τη συγκεκριμένη θέση του πίνακα. |
| [GetEnumerator](../../aspose.tasks/outlinecodedefinitioncollection/getenumerator/)() | Επιστρέφει έναν απαριθμητή για αυτή τη συλλογή. |
| [IndexOf](../../aspose.tasks/outlinecodedefinitioncollection/indexof/)(OutlineCodeDefinition) | Καθορίζει το δείκτη του καθορισμένου στοιχείου σε αυτή τη συλλογή. |
| [Insert](../../aspose.tasks/outlinecodedefinitioncollection/insert/)(int, OutlineCodeDefinition) | Εισάγει το καθορισμένο στοιχείο στον καθορισμένο δείκτη. |
| [Remove](../../aspose.tasks/outlinecodedefinitioncollection/remove/)(OutlineCodeDefinition) | Αφαιρεί την πρώτη εμφάνιση ενός συγκεκριμένου αντικειμένου από αυτή τη συλλογή. |
| [RemoveAt](../../aspose.tasks/outlinecodedefinitioncollection/removeat/)(int) | Αφαιρεί ένα στοιχείο στον καθορισμένο δείκτη. |
| [ToList](../../aspose.tasks/outlinecodedefinitioncollection/tolist/)() | Μετατρέπει αυτό το αντικείμενο OutlineCodeDefinitionCollection σε λίστα αντικειμένων [`OutlineCodeDefinition`](../outlinecodedefinition/). |

## Παραδείγματα

Δείχνει πώς να εργάζεστε με συλλογές ορισμών κώδικα περιγράμματος.

```csharp
var project = new Project(DataDir + "OutlineCodes.mpp");

Console.WriteLine("Count of outline code definitions: " + project.OutlineCodes.Count);
foreach (var outlineCode in project.OutlineCodes)
{
    Console.WriteLine("Field Name: " + outlineCode.FieldName);
    Console.WriteLine("Alias: " + outlineCode.Alias);
    Console.WriteLine();
}

// προσθέστε έναν προσαρμοσμένο ορισμό outline code
var outlineCodeDefinition = new OutlineCodeDefinition { FieldId = ((int)ExtendedAttributeTask.OutlineCode3).ToString("D"), Alias = "My Outline Code" };

var outlineCodeDefinition2 = new OutlineCodeDefinition { FieldId = ((int)ExtendedAttributeTask.OutlineCode1).ToString("D"), Alias = "My Outline Code 2" };

if (!project.OutlineCodes.IsReadOnly)
{
    project.OutlineCodes.Add(outlineCodeDefinition);

    // εισαγωγή ορισμού κώδικα περιγράμματος στη θέση
    project.OutlineCodes.Insert(0, outlineCodeDefinition2);
}

// εύρεση του δείκτη του ορισμού κώδικα περιγράμματος
var index = project.OutlineCodes.IndexOf(outlineCodeDefinition);

// επεξεργαστείτε τον ορισμό κώδικα περιγράμματος
project.OutlineCodes[index].Alias = "New Alias";

// ...
// εργαστείτε με ορισμούς κώδικα περιγράμματος
// ...

// αφαιρέστε τον ορισμό κώδικα περιγράμματος
if (project.OutlineCodes.Contains(outlineCodeDefinition))
{
    project.OutlineCodes.Remove(outlineCodeDefinition);
}

// αφαιρέστε έναν ορισμό κώδικα περιγράμματος με βάση τον δείκτη
project.OutlineCodes.RemoveAt(0);

var otherProject = new Project(DataDir + "Blank2010.mpp");

// αφαιρέστε ορισμούς κώδικα περιγράμματος
otherProject.OutlineCodes.Clear();

// αντιγράψτε ορισμούς κώδικα περιγράμματος
var outlineCodeDefinitions = new OutlineCodeDefinition[project.OutlineCodes.Count];
project.OutlineCodes.CopyTo(outlineCodeDefinitions, 0);

foreach (var definition in outlineCodeDefinitions)
{
    otherProject.OutlineCodes.Add(definition);
}

// ...
// εργαστείτε με ορισμούς κώδικα περιγράμματος
// ...

// αφαιρέστε ορισμούς κώδικα περιγράμματος ένας-ένας
List<OutlineCodeDefinition> definitions = otherProject.OutlineCodes.ToList();
foreach (var definition in definitions)
{
    otherProject.OutlineCodes.Remove(definition);
}
```

### Δείτε επίσης

* class [OutlineCodeDefinition](../outlinecodedefinition/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


