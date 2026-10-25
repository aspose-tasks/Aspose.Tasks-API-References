---
title: "TableCollection.CopyTo"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος TableCollection. Αντιγράφει τα στοιχεία αυτής της συλλογής στον καθορισμένο πίνακα ξεκινώντας από τον καθορισμένο δείκτη του πίνακα"
type: docs
weight: 60
url: /el/net/aspose.tasks/tablecollection/copyto/
---
## TableCollection.CopyTo method

Αντιγράφει τα στοιχεία αυτής της συλλογής στον καθορισμένο πίνακα, ξεκινώντας από τη συγκεκριμένη θέση του πίνακα.

```csharp
public void CopyTo(Table[] array, int arrayIndex)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| array | Table[] | ο καθορισμένος μονοδιάστατος πίνακας για αντιγραφή των στοιχείων σε αυτόν |
| arrayIndex | Int32 | ο μηδενικός δείκτης του καθορισμένου πίνακα στον οποίο αρχίζει η αντιγραφή. |

## Παραδείγματα

Δείχνει πώς να εργαστείτε με συλλογές πινάκων.

```csharp
var project = new Project(DataDir + "Project1.mpp");

Console.WriteLine("Is collection of tables read-only?: " + project.Tables.IsReadOnly);

// επανάληψη στους πίνακες
Console.WriteLine("Print tables of " + project.Get(Prj.Name) + " project.");
Console.WriteLine("Table count: " + project.Tables.Count);
foreach (var tbl in project.Tables)
{
    Console.WriteLine("Name: " + tbl.Name);

    Console.WriteLine("Fields:");

    foreach (var field in tbl.TableFields)
    {
        Console.WriteLine("    {0} - '{1}' - {2}", field.Field, field.Title, field.Width);
    }
}

// προσθέστε έναν νέο πίνακα
var tableToAdd = new Table
{
    Name = "New Table",
    ShowInMenu = true
};
project.Tables.Add(tableToAdd);

Console.WriteLine("The collection contains the new table?: " + project.Tables.Contains(tableToAdd));

// μπορεί κανείς να εκκαθαρίσει τη συλλογή με δύο τρόπους
if (deleteOneByOne)
{
    // αντιγράψτε πίνακες στον πίνακα και διαγράψτε τους έναν-έναν
    var tables = new Table[project.Tables.Count];
    project.Tables.CopyTo(tables, 0);
    foreach (var table in tables)
    {
        project.Tables.Remove(table);
    }
}
else
{
    // ή μπορεί κανείς να εκκαθαρίσει μια συλλογή πινάκων πλήρως
    project.Tables.Clear();
}

// η συλλογή μπορεί να μετατραπεί σε μια απλή λίστα πινάκων
List<Table> list = project.Tables.ToList();
foreach (var table in list)
{
    Console.WriteLine("Name: " + table.Name);
}
```

### Δείτε επίσης

* class [Table](../../table/)
* class [TableCollection](../)
* namespace [Aspose.Tasks](../../tablecollection/)
* assembly [Aspose.Tasks](../../../)


