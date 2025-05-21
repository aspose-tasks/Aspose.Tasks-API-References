---
title: Table.Uid
second_title: Aspose.Tasks for .NET API Reference
description: Table property. Gets the unique identifier of a table
type: docs
weight: 110
url: /net/aspose.tasks/table/uid/
---
## Table.Uid property

Gets the unique identifier of a table.

```csharp
public int Uid { get; }
```

## Examples

Shows how to define a new table (using for views).

```csharp
var project = new Project(DataDir + "Project1.mpp");

// get a table to edit
var table = project.Tables.ToList()[0];
Console.WriteLine("Uid of the table: " + table.Uid);
Console.WriteLine("Name of the table: " + table.Name);
Console.WriteLine("Type of the table: " + table.TableType);

// tune some properties
// set a value indicating whether the header row height of the table can be adjusted
table.AdjustHeaderRowHeight = true;

// set the date format of the table.
table.DateFormat = DateFormat.DateDdMmYyyy;

// set a value indicating whether the first column of a table is locked or editable
table.LockFirstColumn = true;

// set the row height in a table, where the row height is the number of lines of text
table.RowHeight = 10;

// sets a value indicating whether to show 'Add New Column' interface
table.ShowAddNewColumn = true;

// set a value indicating whether project shows the table name in the Tables drop-down list on the View tab of the Ribbon
table.ShowInMenu = true;

// lets save the updated table
project.Save(OutDir + "WorkWithTable_out.mpp", SaveFileFormat.Mpp);
```

### See Also

* class [Table](../)
* namespace [Aspose.Tasks](../../table/)
* assembly [Aspose.Tasks](../../../)


