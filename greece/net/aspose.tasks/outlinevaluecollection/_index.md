---
title: "Κλάση OutlineValueCollection"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.OutlineValueCollection κλάση. Αντιπροσωπεύει μια συλλογή αντικειμένων OutlineValue."
type: docs
weight: 1220
url: /el/net/aspose.tasks/outlinevaluecollection/
---
## OutlineValueCollection class

Αντιπροσωπεύει μια συλλογή αντικειμένων [`OutlineValue`](../outlinevalue/).

```csharp
public class OutlineValueCollection : IList<OutlineValue>
```

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [Count](../../aspose.tasks/outlinevaluecollection/count/) { get; } | Λαμβάνει τον αριθμό των στοιχείων που περιέχονται σε αυτή τη συλλογή. |
| [IsReadOnly](../../aspose.tasks/outlinevaluecollection/isreadonly/) { get; } | Λαμβάνει μια τιμή που υποδεικνύει εάν αυτή η συλλογή είναι μόνο για ανάγνωση. |
| [Item](../../aspose.tasks/outlinevaluecollection/item/) { get; set; } | Επιστρέφει ή ορίζει το στοιχείο στη συγκεκριμένη θέση. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| [Add](../../aspose.tasks/outlinevaluecollection/add/)(OutlineValue) | Προσθέτει το καθορισμένο στοιχείο σε αυτή τη συλλογή. |
| [Clear](../../aspose.tasks/outlinevaluecollection/clear/)() | Αφαιρεί όλα τα στοιχεία από αυτή τη συλλογή. |
| [Contains](../../aspose.tasks/outlinevaluecollection/contains/)(OutlineValue) | Επιστρέφει true εάν το καθορισμένο στοιχείο βρεθεί σε αυτή τη συλλογή· διαφορετικά, false. |
| [CopyTo](../../aspose.tasks/outlinevaluecollection/copyto/)(OutlineValue[], int) | Αντιγράφει τα στοιχεία αυτής της συλλογής στον καθορισμένο πίνακα, ξεκινώντας από τη συγκεκριμένη θέση του πίνακα. |
| [GetEnumerator](../../aspose.tasks/outlinevaluecollection/getenumerator/)() | Επιστρέφει έναν απαριθμητή για αυτή τη συλλογή. |
| [IndexOf](../../aspose.tasks/outlinevaluecollection/indexof/)(OutlineValue) | Καθορίζει το δείκτη του καθορισμένου στοιχείου σε αυτή τη συλλογή. |
| [Insert](../../aspose.tasks/outlinevaluecollection/insert/)(int, OutlineValue) | Εισάγει το καθορισμένο στοιχείο στον καθορισμένο δείκτη. |
| [Remove](../../aspose.tasks/outlinevaluecollection/remove/)(OutlineValue) | Αφαιρεί την πρώτη εμφάνιση ενός συγκεκριμένου αντικειμένου από αυτή τη συλλογή. |
| [RemoveAt](../../aspose.tasks/outlinevaluecollection/removeat/)(int) | Αφαιρεί ένα στοιχείο στον καθορισμένο δείκτη. |

## Παραδείγματα

Δείχνει πώς να εργαστείτε με συλλογές τιμών περιγράμματος.

```csharp
var project = new Project(DataDir + "OutlineValues2010.mpp");

// καθαρισμός συλλογών τιμών
foreach (var outlineCode in project.OutlineCodes)
{
    // καθαρισμός μάσκων περιγράμματος
    if (outlineCode.Values.Count <= 0)
    {
        continue;
    }

    if (!outlineCode.Values.IsReadOnly)
    {
        outlineCode.Values.Clear();
    }
}

var codeDefinition = new OutlineCodeDefinition
                         {
                             Alias = "New task outline code1", FieldId = ((int)ExtendedAttributeTask.OutlineCode1).ToString(), FieldName = "Outline Code1"
                         };
var value = new OutlineValue { Description = "Value description", ValueId = 1, Value = "123456", Type = OutlineValueType.Number };
codeDefinition.Values.Add(value);
project.OutlineCodes.Add(codeDefinition);

// ενημέρωση τιμής μέσω πρόσβασης δείκτη
codeDefinition.Values[0].Value = "654321";

// επανάληψη πάνω από τιμές περιγράμματος
foreach (var definitionValue in codeDefinition.Values)
{
    Console.WriteLine("Value: " + definitionValue.Value);
    Console.WriteLine("Value Id: " + definitionValue.ValueId);
    Console.WriteLine("Value Guid: " + definitionValue.ValueGuid);
    Console.WriteLine();
}

// ...
// εργασία με τιμές περιγράμματος
// ...

// αφαίρεση τιμής όταν χρειάζεται
if (codeDefinition.Values.Contains(value))
{
    codeDefinition.Values.Remove(value);
}

// εισαγωγή τιμής στη θέση έναρξης
codeDefinition.Values.Insert(0, value);

// έλεγχος της θέσης της εισαχθείσας τιμής
Console.WriteLine("Index of inserted value: " + codeDefinition.Values.IndexOf(value));

// ...
// εργασία με τιμές περιγράμματος
// ...

// αφαίρεση της τελευταίας τιμής από τη συλλογή
codeDefinition.Values.RemoveAt(codeDefinition.Values.Count - 1);

// μπορεί κανείς να δημιουργήσει έναν άλλο ορισμό κώδικα περιγράμματος
var codeDefinition2 = new OutlineCodeDefinition
                          {
                              Alias = "New outline code 2", FieldId = ((int)ExtendedAttributeTask.OutlineCode2).ToString(), FieldName = "Outline Code2"
                          };

// και στη συνέχεια αντιγραφή τιμών περιγράμματος
var outlineValues = new OutlineValue[codeDefinition.Values.Count];
codeDefinition.Values.CopyTo(outlineValues, 0);

foreach (var outlineValue in outlineValues)
{
    codeDefinition2.Values.Add(outlineValue);
}
```

### Δείτε επίσης

* class [OutlineValue](../outlinevalue/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


