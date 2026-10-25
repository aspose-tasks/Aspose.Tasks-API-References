---
title: "TableFieldCollection.Insert"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "TableFieldCollection-methode. Voegt het opgegeven item in op de opgegeven index"
type: docs
weight: 100
url: /nl/net/aspose.tasks/tablefieldcollection/insert/
---
## TableFieldCollection.Insert method

Voegt het opgegeven item in op de opgegeven index.

```csharp
public void Insert(int index, TableField item)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| index | Int32 | de opgegeven nulgebaseerde index waarop het item moet worden ingevoegd. |
| item | TableField | het opgegeven item om in deze collectie in te voegen. |

## Voorbeelden

Toont hoe te werken met tabelveldcollecties.

```csharp
var project = new Project(DataDir + "Project1.mpp");

foreach (var tbl in project.Tables)
{
    Console.WriteLine("Table name: " + tbl.Name);
    Console.WriteLine("Is collection of table fields read-only?: " + tbl.TableFields.IsReadOnly);

    // itereren over tabelvelden
    Console.WriteLine("Print table fields of " + project.Get(Prj.Name) + " project.");
    Console.WriteLine("Table count: " + tbl.TableFields.Count);
    foreach (var fld in tbl.TableFields)
    {
        Console.WriteLine("Field Title: " + fld.Title);
        Console.WriteLine("Field Field: " + fld.Field);
        Console.WriteLine();
    }
}

// voeg een nieuw tabelveld toe
var table = project.Tables.ToList()[0];
var field = new TableField();
field.Title = "New Table Field";
table.TableFields.Add(field);

var field2 = new TableField();
field2.Title = "New Table Field 2";

// voeg een nieuw veld in op de positie
var idx = table.TableFields.IndexOf(field);
table.TableFields.Insert(idx, field2);

// laat ons het nieuwe tabelveld bewerken door indextoegang te gebruiken
table.TableFields[idx].WrapHeader = true;

Console.WriteLine("The collection contains the new table field?: " + table.TableFields.Contains(field));

// recentelijk kunnen we het veld verwijderen
table.TableFields.RemoveAt(idx);

// men kan de collectie op twee manieren wissen
if (deleteOneByOne)
{
    // kopieer tabelvelden naar de array en verwijder ze één voor één
    var tableFields = new TableField[table.TableFields.Count];
    table.TableFields.CopyTo(tableFields, 0);
    foreach (var fld in tableFields)
    {
        table.TableFields.Remove(fld);
    }
}
else
{
    // of men kan een tabelveldcollectie volledig wissen
    table.TableFields.Clear();
}
```

### Zie ook

* class [TableField](../../tablefield/)
* class [TableFieldCollection](../)
* namespace [Aspose.Tasks](../../tablefieldcollection/)
* assembly [Aspose.Tasks](../../../)


