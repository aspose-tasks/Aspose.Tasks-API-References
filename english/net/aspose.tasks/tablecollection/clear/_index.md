---
title: TableCollection.Clear
second_title: Aspose.Tasks for .NET API Reference
description: TableCollection method. Removes all items from this collection
type: docs
weight: 40
url: /net/aspose.tasks/tablecollection/clear/
---
## TableCollection.Clear method

Removes all items from this collection.

```csharp
public void Clear()
```

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
    Console.WriteLine("Index: " + tbl.Index);
    Console.WriteLine("Name: " + tbl.Name);
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
    Console.WriteLine("Index: " + table.Index);
    Console.WriteLine("Name: " + table.Name);
}
```

### See Also

* class [TableCollection](../)
* namespace [Aspose.Tasks](../../tablecollection/)
* assembly [Aspose.Tasks](../../../)


