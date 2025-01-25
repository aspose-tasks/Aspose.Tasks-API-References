---
title: Table.Equals
second_title: Aspose.Tasks for .NET API Reference
description: Table method. Returns a value indicating whether this instance is equal to a specified object
type: docs
weight: 120
url: /net/aspose.tasks/table/equals/
---
## Table.Equals method

Returns a value indicating whether this instance is equal to a specified object.

```csharp
public override bool Equals(object obj)
```

| Parameter | Type | Description |
| --- | --- | --- |
| obj | Object | The object to compare with this instance. |

### Return Value

**True** if the specified object is a Table that has the same UID value as this instance; otherwise, **false**.

## Examples

Shows how to check table equality.

```csharp
var project = new Project(DataDir + "ReadFilterDefinitionData.mpp");
List<Table> tables = project.Tables.ToList();

var table1 = tables[0];
var table2 = tables[1];

// the equality of tables is checked against to table's UID.
Console.WriteLine("Table 1 UID: " + table1.Uid);
Console.WriteLine("Table 2 UID: " + table2.Uid);
Console.WriteLine("Are tables equal: " + table1.Equals(table2));
```

### See Also

* class [Table](../)
* namespace [Aspose.Tasks](../../table/)
* assembly [Aspose.Tasks](../../../)


