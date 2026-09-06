---
title: "TableCollection.Clear"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode TableCollection. Supprime tous les éléments de cette collection"
type: docs
weight: 40
url: /fr/net/aspose.tasks/tablecollection/clear/
---
## TableCollection.Clear method

Supprime tous les éléments de cette collection.

```csharp
public void Clear()
```

## Exemples

Montre comment travailler avec les collections de tables.

```csharp
var project = new Project(DataDir + "Project1.mpp");

Console.WriteLine("Is collection of tables read-only?: " + project.Tables.IsReadOnly);

// parcourir les tables
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

// ajouter une nouvelle table
var tableToAdd = new Table
{
    Name = "New Table",
    ShowInMenu = true
};
project.Tables.Add(tableToAdd);

Console.WriteLine("The collection contains the new table?: " + project.Tables.Contains(tableToAdd));

// on peut vider la collection de deux manières
if (deleteOneByOne)
{
    // copier les tables dans le tableau et les supprimer une par une
    var tables = new Table[project.Tables.Count];
    project.Tables.CopyTo(tables, 0);
    foreach (var table in tables)
    {
        project.Tables.Remove(table);
    }
}
else
{
    // ou on peut vider complètement une collection de tables
    project.Tables.Clear();
}

// la collection peut être convertie en une simple liste de tables
List<Table> list = project.Tables.ToList();
foreach (var table in list)
{
    Console.WriteLine("Name: " + table.Name);
}
```

### Voir aussi

* class [TableCollection](../)
* namespace [Aspose.Tasks](../../tablecollection/)
* assembly [Aspose.Tasks](../../../)


