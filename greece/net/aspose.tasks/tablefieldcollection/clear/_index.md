---
title: "TableFieldCollection.Clear"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "TableFieldCollection μέθοδος. Αφαιρεί όλα τα στοιχεία από αυτή τη συλλογή"
type: docs
weight: 50
url: /el/net/aspose.tasks/tablefieldcollection/clear/
---
## TableFieldCollection.Clear method

Αφαιρεί όλα τα στοιχεία από αυτή τη συλλογή.

```csharp
public void Clear()
```

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

* class [TableFieldCollection](../)
* namespace [Aspose.Tasks](../../tablefieldcollection/)
* assembly [Aspose.Tasks](../../../)


