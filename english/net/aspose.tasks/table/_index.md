---
title: Class Table
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.Table class. Represents a table in Project
type: docs
weight: 2290
url: /net/aspose.tasks/table/
---
## Table class

Represents a table in Project

```csharp
public class Table
```

## Constructors

| Name | Description |
| --- | --- |
| [Table](table/)() | Initializes a new instance of the `Table` class. |

## Properties

| Name | Description |
| --- | --- |
| [AdjustHeaderRowHeight](../../aspose.tasks/table/adjustheaderrowheight/) { get; set; } | Gets or sets a value indicating whether the header row height of the table can be adjusted. |
| [DateFormat](../../aspose.tasks/table/dateformat/) { get; set; } | Gets or sets the date format of the table. |
| [LockFirstColumn](../../aspose.tasks/table/lockfirstcolumn/) { get; set; } | Gets or sets a value indicating whether the first column of a table is locked or editable. |
| [Name](../../aspose.tasks/table/name/) { get; set; } | Gets or sets the name of a Table object. |
| [RowHeight](../../aspose.tasks/table/rowheight/) { get; set; } | Gets or sets the row height in a table, where the row height is the number of lines of text. |
| [ShowAddNewColumn](../../aspose.tasks/table/showaddnewcolumn/) { get; set; } | Gets or sets a value indicating whether to show 'Add New Column' interface. Supported by MSP 2010 version and later. |
| [ShowInMenu](../../aspose.tasks/table/showinmenu/) { get; set; } | Gets or sets a value indicating whether project shows the table name in the Tables drop-down list on the View tab of the Ribbon. |
| [TableFields](../../aspose.tasks/table/tablefields/) { get; } | Gets a TableFields collection representing the fields in the table. |
| [TableType](../../aspose.tasks/table/tabletype/) { get; set; } | Gets or sets the table type for the specified table. |
| [Uid](../../aspose.tasks/table/uid/) { get; } | Gets the unique identifier of a table. |

## Methods

| Name | Description |
| --- | --- |
| override [Equals](../../aspose.tasks/table/equals/)(object) | Returns a value indicating whether this instance is equal to a specified object. |
| override [GetHashCode](../../aspose.tasks/table/gethashcode/)() | Returns a hash code for this Table. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


