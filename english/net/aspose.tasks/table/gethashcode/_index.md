---
title: Table.GetHashCode
second_title: Aspose.Tasks for .NET API Reference
description: Table method. Returns a hash code for this Table
type: docs
weight: 130
url: /net/aspose.tasks/table/gethashcode/
---
## Table.GetHashCode method

Returns a hash code for this Table.

```csharp
public override int GetHashCode()
```

### Return Value

Returns a hash code value for this object.

## Examples

Shows how to get a hash code of a table.

```csharp
var project = new Project(DataDir + "ReadFilterDefinitionData.mpp");

List<Table> tables = project.Tables.ToList();

var table1 = tables[0];
var table2 = tables[1];

// the hash code of a table is equal to table UID 
Console.WriteLine("Table UID: {0} Hash Code: {1}", table1.Uid, table1.GetHashCode());
Console.WriteLine("Table UID: {0} Hash Code: {1}", table2.Uid, table2.GetHashCode());
```

### See Also

* class [Table](../)
* namespace [Aspose.Tasks](../../table/)
* assembly [Aspose.Tasks](../../../)


