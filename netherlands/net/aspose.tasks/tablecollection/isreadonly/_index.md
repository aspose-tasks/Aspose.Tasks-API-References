---
title: "TableCollection.IsReadOnly"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "TableCollection-eigenschap. Haalt een waarde op die aangeeft of deze collectie alleen-lezen is, anders false"
type: docs
weight: 20
url: /nl/net/aspose.tasks/tablecollection/isreadonly/
---
## TableCollection.IsReadOnly property

Haalt een waarde op die aangeeft of deze collectie alleen-lezen is; anders, false.

```csharp
public bool IsReadOnly { get; }
```

## Voorbeelden

Toont hoe te werken met tabelcollecties.

```csharp
var project = new Project(DataDir + "Project1.mpp");

Console.WriteLine("Is collection of tables read-only?: " + project.Tables.IsReadOnly);

// itereren over tabellen
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

// voeg een nieuwe tabel toe
var tableToAdd = new Table
{
    Name = "New Table",
    ShowInMenu = true
};
project.Tables.Add(tableToAdd);

Console.WriteLine("The collection contains the new table?: " + project.Tables.Contains(tableToAdd));

// men kan de collectie op twee manieren wissen
if (deleteOneByOne)
{
    // kopieer tabellen naar de array en verwijder ze één voor één
    var tables = new Table[project.Tables.Count];
    project.Tables.CopyTo(tables, 0);
    foreach (var table in tables)
    {
        project.Tables.Remove(table);
    }
}
else
{
    // of men kan een tabelcollectie volledig wissen
    project.Tables.Clear();
}

// de collectie kan worden omgezet in een eenvoudige lijst met tabellen
List<Table> list = project.Tables.ToList();
foreach (var table in list)
{
    Console.WriteLine("Name: " + table.Name);
}
```

### Zie ook

* class [TableCollection](../)
* namespace [Aspose.Tasks](../../tablecollection/)
* assembly [Aspose.Tasks](../../../)


