---
title: Class TableCollection
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.TableCollection class. Contains a list of Table objects. Implements ICollectionTable interface
type: docs
weight: 2300
url: /net/aspose.tasks/tablecollection/
---
## TableCollection class

Contains a list of [`Table`](../table/) objects. Implements ICollection&lt;Table&gt; interface.

```csharp
public class TableCollection : ICollection<Table>
```

## Properties

| Name | Description |
| --- | --- |
| [Count](../../aspose.tasks/tablecollection/count/) { get; } | Gets the number of elements contained in this collection. |
| [IsReadOnly](../../aspose.tasks/tablecollection/isreadonly/) { get; } | Gets a value indicating whether this collection is read-only; otherwise, false. |

## Methods

| Name | Description |
| --- | --- |
| [Add](../../aspose.tasks/tablecollection/add/)(Table) | Adds the specified item to this collection. |
| [Clear](../../aspose.tasks/tablecollection/clear/)() | Removes all items from this collection. |
| [Contains](../../aspose.tasks/tablecollection/contains/)(Table) | Returns true if the specified item is found in this collection; otherwise, false. |
| [CopyTo](../../aspose.tasks/tablecollection/copyto/)(Table[], int) | Copies the elements of this collection to the specified array, starting at the specified array index. |
| [GetEnumerator](../../aspose.tasks/tablecollection/getenumerator/)() | Returns an enumerator for this collection. |
| [Remove](../../aspose.tasks/tablecollection/remove/)(Table) | Removes the first occurrence of a specific object from this collection. |
| [ToList](../../aspose.tasks/tablecollection/tolist/)() | Converts a table collection to a list of [`Table`](../table/) objects. |

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

* class [Table](../table/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


