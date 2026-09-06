---
title: "Table.Equals"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Table 方法。返回一个值，指示此实例是否等于指定的对象"
type: docs
weight: 120
url: /zh/net/aspose.tasks/table/equals/
---
## Table.Equals method

返回一个值，指示此实例是否等于指定的对象。

```csharp
public override bool Equals(object obj)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| obj | 对象 | 与此实例比较的对象。 |

### 返回值

**True** if the specified object is a Table that has the same UID value as this instance; otherwise, **false**.

## 示例

展示如何检查表格相等性。

```csharp
var project = new Project(DataDir + "ReadFilterDefinitionData.mpp");
List<Table> tables = project.Tables.ToList();

var table1 = tables[0];
var table2 = tables[1];

// 表格的相等性是根据表的 UID 进行检查的。
Console.WriteLine("Table 1 UID: " + table1.Uid);
Console.WriteLine("Table 2 UID: " + table2.Uid);
Console.WriteLine("Are tables equal: " + table1.Equals(table2));
```

### 另见

* class [Table](../)
* namespace [Aspose.Tasks](../../table/)
* assembly [Aspose.Tasks](../../../)


