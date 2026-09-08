---
title: "Klasse TableCollection"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.TableCollection klasse. Bevat een lijst met Table-objecten. Implementeert de ICollectionTable interface"
type: docs
weight: 2330
url: /nl/net/aspose.tasks/tablecollection/
---
## TableCollection class

Bevat een lijst met [`Table`](../table/) objecten. Implementeert de ICollection&lt;Table&gt; interface.

```csharp
public class TableCollection : ICollection<Table>
```

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [Count](../../aspose.tasks/tablecollection/count/) { get; } | Haalt het aantal elementen op dat in deze collectie zit. |
| [IsReadOnly](../../aspose.tasks/tablecollection/isreadonly/) { get; } | Haalt een waarde op die aangeeft of deze collectie alleen-lezen is; anders, false. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| [Add](../../aspose.tasks/tablecollection/add/)(Table) | Voegt het opgegeven item toe aan deze collectie. |
| [Clear](../../aspose.tasks/tablecollection/clear/)() | Verwijdert alle items uit deze collectie. |
| [Contains](../../aspose.tasks/tablecollection/contains/)(Table) | Retourneert true als het opgegeven item in deze collectie wordt gevonden; anders false. |
| [CopyTo](../../aspose.tasks/tablecollection/copyto/)(Table[], int) | Kopieert de elementen van deze collectie naar de opgegeven array, beginnend bij de opgegeven array-index. |
| [GetEnumerator](../../aspose.tasks/tablecollection/getenumerator/)() | Retourneert een enumerator voor deze collectie. |
| [Remove](../../aspose.tasks/tablecollection/remove/)(Table) | Verwijdert de eerste instantie van een specifiek object uit deze collectie. |
| [ToList](../../aspose.tasks/tablecollection/tolist/)() | Converteert een tabelcollectie naar een lijst met [`Table`](../table/) objecten. |

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

* class [Table](../table/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


