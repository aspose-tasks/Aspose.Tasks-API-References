---
title: "Κλάση TableFieldCollection"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κλάση Aspose.Tasks.TableFieldCollection. Περιέχει μια λίστα αντικειμένων TableField. Υλοποιεί τη διεπαφή IListTableField."
type: docs
weight: 2350
url: /el/net/aspose.tasks/tablefieldcollection/
---
## TableFieldCollection class

Περιέχει μια λίστα αντικειμένων [`TableField`](../tablefield/). Υλοποιεί τη διεπαφή IList&lt;TableField&gt;.

```csharp
public class TableFieldCollection : IList<TableField>
```

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [Count](../../aspose.tasks/tablefieldcollection/count/) { get; } | Λαμβάνει τον αριθμό των στοιχείων που περιέχονται σε αυτή τη συλλογή. |
| [IsReadOnly](../../aspose.tasks/tablefieldcollection/isreadonly/) { get; } | Λαμβάνει μια τιμή που υποδεικνύει εάν αυτή η συλλογή είναι μόνο για ανάγνωση· διαφορετικά, false. |
| [Item](../../aspose.tasks/tablefieldcollection/item/) { get; set; } | Επιστρέφει ή ορίζει το στοιχείο στη συγκεκριμένη θέση. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| [Add](../../aspose.tasks/tablefieldcollection/add/)(TableField) | Προσθέτει το καθορισμένο στοιχείο σε αυτή τη συλλογή. |
| [Clear](../../aspose.tasks/tablefieldcollection/clear/)() | Αφαιρεί όλα τα στοιχεία από αυτή τη συλλογή. |
| [Contains](../../aspose.tasks/tablefieldcollection/contains/)(TableField) | Επιστρέφει true εάν το καθορισμένο στοιχείο βρεθεί σε αυτή τη συλλογή· διαφορετικά, false. |
| [CopyTo](../../aspose.tasks/tablefieldcollection/copyto/)(TableField[], int) | Αντιγράφει τα στοιχεία αυτής της συλλογής στον καθορισμένο πίνακα, ξεκινώντας από τη συγκεκριμένη θέση του πίνακα. |
| [GetEnumerator](../../aspose.tasks/tablefieldcollection/getenumerator/)() | Επιστρέφει έναν απαριθμητή για αυτή τη συλλογή. |
| [IndexOf](../../aspose.tasks/tablefieldcollection/indexof/)(TableField) | Καθορίζει το δείκτη του καθορισμένου στοιχείου σε αυτή τη συλλογή. |
| [Insert](../../aspose.tasks/tablefieldcollection/insert/)(int, TableField) | Εισάγει το καθορισμένο στοιχείο στον καθορισμένο δείκτη. |
| [Remove](../../aspose.tasks/tablefieldcollection/remove/)(TableField) | Αφαιρεί την πρώτη εμφάνιση ενός συγκεκριμένου αντικειμένου από αυτή τη συλλογή. |
| [RemoveAt](../../aspose.tasks/tablefieldcollection/removeat/)(int) | Αφαιρεί ένα στοιχείο στον καθορισμένο δείκτη. |

## Παραδείγματα

Δείχνει πώς να εργαστείτε με συλλογές πεδίων πίνακα.

```csharp
var project = new Project(DataDir + "Project1.mpp");

foreach (var tbl in project.Tables)
{
    Console.WriteLine("Table name: " + tbl.Name);
    Console.WriteLine("Is collection of table fields read-only?: " + tbl.TableFields.IsReadOnly);

    // επανάληψη πάνω από τα πεδία του πίνακα
    Console.WriteLine("Print table fields of " + project.Get(Prj.Name) + " project.");
    Console.WriteLine("Table count: " + tbl.TableFields.Count);
    foreach (var fld in tbl.TableFields)
    {
        Console.WriteLine("Field Title: " + fld.Title);
        Console.WriteLine("Field Field: " + fld.Field);
        Console.WriteLine();
    }
}

// προσθήκη νέου πεδίου πίνακα
var table = project.Tables.ToList()[0];
var field = new TableField();
field.Title = "New Table Field";
table.TableFields.Add(field);

var field2 = new TableField();
field2.Title = "New Table Field 2";

// εισαγωγή νέου πεδίου στη θέση
var idx = table.TableFields.IndexOf(field);
table.TableFields.Insert(idx, field2);

// επιτρέπει την επεξεργασία του νέου πεδίου πίνακα χρησιμοποιώντας πρόσβαση με δείκτη
table.TableFields[idx].WrapHeader = true;

Console.WriteLine("The collection contains the new table field?: " + table.TableFields.Contains(field));

// πρόσφατα μπορούμε να αφαιρέσουμε το πεδίο
table.TableFields.RemoveAt(idx);

// μπορεί κανείς να εκκαθαρίσει τη συλλογή με δύο τρόπους
if (deleteOneByOne)
{
    // αντιγράψτε τα πεδία του πίνακα στον πίνακα και διαγράψτε τα ένα-ένα
    var tableFields = new TableField[table.TableFields.Count];
    table.TableFields.CopyTo(tableFields, 0);
    foreach (var fld in tableFields)
    {
        table.TableFields.Remove(fld);
    }
}
else
{
    // ή μπορεί κανείς να καθαρίσει πλήρως μια συλλογή πεδίων πίνακα
    table.TableFields.Clear();
}
```

### Δείτε επίσης

* class [TableField](../tablefield/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


