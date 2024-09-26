---
title: TableFieldCollection.GetEnumerator
second_title: Aspose.Tasks for .NET API Reference
description: TableFieldCollection method. Returns an enumerator for this collection
type: docs
weight: 80
url: /net/aspose.tasks/tablefieldcollection/getenumerator/
---
## TableFieldCollection.GetEnumerator method

Returns an enumerator for this collection.

```csharp
public IEnumerator<TableField> GetEnumerator()
```

### Return Value

an enumerator for this collection.

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

* class [TableField](../../tablefield/)
* class [TableFieldCollection](../)
* namespace [Aspose.Tasks](../../tablefieldcollection/)
* assembly [Aspose.Tasks](../../../)


