---
title: "TableFieldCollection.RemoveAt"
second_title: "Aspose.Tasks for .NET API 参考"
description: "TableFieldCollection 方法。移除指定索引处的项"
type: docs
weight: 120
url: /zh/net/aspose.tasks/tablefieldcollection/removeat/
---
## TableFieldCollection.RemoveAt method

在指定索引处移除一项。

```csharp
public void RemoveAt(int index)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| index | Int32 | 要在其移除项的指定零基索引。 |

## 示例

展示如何使用表字段集合。

```csharp
var project = new Project(DataDir + "Project1.mpp");

foreach (var tbl in project.Tables)
{
    Console.WriteLine("Table name: " + tbl.Name);
    Console.WriteLine("Is collection of table fields read-only?: " + tbl.TableFields.IsReadOnly);

    // 遍历表字段
    Console.WriteLine("Print table fields of " + project.Get(Prj.Name) + " project.");
    Console.WriteLine("Table count: " + tbl.TableFields.Count);
    foreach (var fld in tbl.TableFields)
    {
        Console.WriteLine("Field Title: " + fld.Title);
        Console.WriteLine("Field Field: " + fld.Field);
        Console.WriteLine();
    }
}

// 添加一个新表字段
var table = project.Tables.ToList()[0];
var field = new TableField();
field.Title = "New Table Field";
table.TableFields.Add(field);

var field2 = new TableField();
field2.Title = "New Table Field 2";

// 在指定位置插入新字段
var idx = table.TableFields.IndexOf(field);
table.TableFields.Insert(idx, field2);

// 通过索引访问编辑新表字段
table.TableFields[idx].WrapHeader = true;

Console.WriteLine("The collection contains the new table field?: " + table.TableFields.Contains(field));

// 最近我们可以删除该字段
table.TableFields.RemoveAt(idx);

// 可以通过两种方式清除集合
if (deleteOneByOne)
{
    // 将表字段复制到数组中并逐个删除
    var tableFields = new TableField[table.TableFields.Count];
    table.TableFields.CopyTo(tableFields, 0);
    foreach (var fld in tableFields)
    {
        table.TableFields.Remove(fld);
    }
}
else
{
    // 或者可以完全清空表字段集合
    table.TableFields.Clear();
}
```

### 另见

* class [TableFieldCollection](../)
* namespace [Aspose.Tasks](../../tablefieldcollection/)
* assembly [Aspose.Tasks](../../../)


