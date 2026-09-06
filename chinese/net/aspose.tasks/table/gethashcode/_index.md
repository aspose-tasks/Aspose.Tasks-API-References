---
title: "Table.GetHashCode"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Table 方法。返回此 Table 的哈希码"
type: docs
weight: 130
url: /zh/net/aspose.tasks/table/gethashcode/
---
## Table.GetHashCode method

返回此表的哈希码。

```csharp
public override int GetHashCode()
```

### 返回值

返回此对象的哈希码值。

## 示例

展示如何获取表格的哈希码。

```csharp
var project = new Project(DataDir + "ReadFilterDefinitionData.mpp");

List<Table> tables = project.Tables.ToList();

var table1 = tables[0];
var table2 = tables[1];

// 表格的哈希码等于表的 UID。
Console.WriteLine("Table UID: {0} Hash Code: {1}", table1.Uid, table1.GetHashCode());
Console.WriteLine("Table UID: {0} Hash Code: {1}", table2.Uid, table2.GetHashCode());
```

### 另见

* class [Table](../)
* namespace [Aspose.Tasks](../../table/)
* assembly [Aspose.Tasks](../../../)


