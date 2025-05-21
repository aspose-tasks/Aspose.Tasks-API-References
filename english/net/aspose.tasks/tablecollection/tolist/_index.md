---
title: TableCollection.ToList
second_title: Aspose.Tasks for .NET API Reference
description: TableCollection method. Converts a table collection to a list of Table objects
type: docs
weight: 90
url: /net/aspose.tasks/tablecollection/tolist/
---
## TableCollection.ToList method

Converts a table collection to a list of [`Table`](../../table/) objects.

```csharp
public List<Table> ToList()
```

### Return Value

Generic list of [`Table`](../../table/) objects.

## Examples

Shows how to work with table collections.

```csharp
var project = new Project(DataDir + "Project1.mpp");

Console.WriteLine("Is collection of tables read-only?: " + project.Tables.IsReadOnly);

// iterate over tables
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

// add a new table
var tableToAdd = new Table
{
    Name = "New Table",
    ShowInMenu = true
};
project.Tables.Add(tableToAdd);

Console.WriteLine("The collection contains the new table?: " + project.Tables.Contains(tableToAdd));

// one can clear the collection in two ways
if (deleteOneByOne)
{
    // copy tables into the array and delete them one by one
    var tables = new Table[project.Tables.Count];
    project.Tables.CopyTo(tables, 0);
    foreach (var table in tables)
    {
        project.Tables.Remove(table);
    }
}
else
{
    // or one can clear a table collection completely
    project.Tables.Clear();
}

// the collection can be converted into a plain list of tables
List<Table> list = project.Tables.ToList();
foreach (var table in list)
{
    Console.WriteLine("Name: " + table.Name);
}
```

### See Also

* class [Table](../../table/)
* class [TableCollection](../)
* namespace [Aspose.Tasks](../../tablecollection/)
* assembly [Aspose.Tasks](../../../)


