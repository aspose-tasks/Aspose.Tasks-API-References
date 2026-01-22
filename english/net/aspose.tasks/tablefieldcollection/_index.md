---
title: Class TableFieldCollection
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.TableFieldCollection class. Contains a list of TableField objects. Implements IListTableField interface
type: docs
weight: 2320
url: /net/aspose.tasks/tablefieldcollection/
---
## TableFieldCollection class

Contains a list of [`TableField`](../tablefield/) objects. Implements IList&lt;TableField&gt; interface.

```csharp
public class TableFieldCollection : IList<TableField>
```

## Properties

| Name | Description |
| --- | --- |
| [Count](../../aspose.tasks/tablefieldcollection/count/) { get; } | Gets the number of elements contained in this collection. |
| [IsReadOnly](../../aspose.tasks/tablefieldcollection/isreadonly/) { get; } | Gets a value indicating whether this collection is read-only; otherwise, false. |
| [Item](../../aspose.tasks/tablefieldcollection/item/) { get; set; } | Returns or sets the element at the specified index. |

## Methods

| Name | Description |
| --- | --- |
| [Add](../../aspose.tasks/tablefieldcollection/add/)(TableField) | Adds the specified item to this collection. |
| [Clear](../../aspose.tasks/tablefieldcollection/clear/)() | Removes all items from this collection. |
| [Contains](../../aspose.tasks/tablefieldcollection/contains/)(TableField) | Returns true if the specified item is found in this collection; otherwise, false. |
| [CopyTo](../../aspose.tasks/tablefieldcollection/copyto/)(TableField[], int) | Copies the elements of this collection to the specified array, starting at the specified array index. |
| [GetEnumerator](../../aspose.tasks/tablefieldcollection/getenumerator/)() | Returns an enumerator for this collection. |
| [IndexOf](../../aspose.tasks/tablefieldcollection/indexof/)(TableField) | Determines the index of the specified item in this collection. |
| [Insert](../../aspose.tasks/tablefieldcollection/insert/)(int, TableField) | Inserts the specified item at the specified index. |
| [Remove](../../aspose.tasks/tablefieldcollection/remove/)(TableField) | Removes the first occurrence of a specific object from this collection. |
| [RemoveAt](../../aspose.tasks/tablefieldcollection/removeat/)(int) | Removes an item at the specified index. |

## Examples

Shows how to work with table field collections.

```csharp
var project = new Project(DataDir + "Project1.mpp");

foreach (var tbl in project.Tables)
{
    Console.WriteLine("Table name: " + tbl.Name);
    Console.WriteLine("Is collection of table fields read-only?: " + tbl.TableFields.IsReadOnly);

    // iterate over table fields
    Console.WriteLine("Print table fields of " + project.Get(Prj.Name) + " project.");
    Console.WriteLine("Table count: " + tbl.TableFields.Count);
    foreach (var fld in tbl.TableFields)
    {
        Console.WriteLine("Field Title: " + fld.Title);
        Console.WriteLine("Field Field: " + fld.Field);
        Console.WriteLine();
    }
}

// add a new table field
var table = project.Tables.ToList()[0];
var field = new TableField();
field.Title = "New Table Field";
table.TableFields.Add(field);

var field2 = new TableField();
field2.Title = "New Table Field 2";

// insert a new field in the position
var idx = table.TableFields.IndexOf(field);
table.TableFields.Insert(idx, field2);

// lets edit the new table field by using index access
table.TableFields[idx].WrapHeader = true;

Console.WriteLine("The collection contains the new table field?: " + table.TableFields.Contains(field));

// lately we can remove the field
table.TableFields.RemoveAt(idx);

// one can clear the collection in two ways
if (deleteOneByOne)
{
    // copy table fields into the array and delete them one by one
    var tableFields = new TableField[table.TableFields.Count];
    table.TableFields.CopyTo(tableFields, 0);
    foreach (var fld in tableFields)
    {
        table.TableFields.Remove(fld);
    }
}
else
{
    // or one can clear a table field collection completely
    table.TableFields.Clear();
}
```

### See Also

* class [TableField](../tablefield/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


