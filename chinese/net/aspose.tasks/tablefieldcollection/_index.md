---
title: "类 TableFieldCollection"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.TableFieldCollection 类。包含 TableField 对象的列表。实现 IListTableField 接口"
type: docs
weight: 2350
url: /zh/net/aspose.tasks/tablefieldcollection/
---
## TableFieldCollection class

包含一个 [`TableField`](../tablefield/) 对象列表。实现 IList&lt;TableField&gt; 接口。

```csharp
public class TableFieldCollection : IList<TableField>
```

## 属性

| 名称 | 描述 |
| --- | --- |
| [Count](../../aspose.tasks/tablefieldcollection/count/) { get; } | 获取此集合中包含的元素数量。 |
| [IsReadOnly](../../aspose.tasks/tablefieldcollection/isreadonly/) { get; } | 获取一个值，指示此集合是否为只读；否则为 false。 |
| [Item](../../aspose.tasks/tablefieldcollection/item/) { get; set; } | 返回或设置指定索引处的元素。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| [Add](../../aspose.tasks/tablefieldcollection/add/)(TableField) | 将指定项添加到此集合中。 |
| [Clear](../../aspose.tasks/tablefieldcollection/clear/)() | 从此集合中移除所有项。 |
| [Contains](../../aspose.tasks/tablefieldcollection/contains/)(TableField) | 如果在此集合中找到指定项则返回 true；否则返回 false。 |
| [CopyTo](../../aspose.tasks/tablefieldcollection/copyto/)(TableField[], int) | 将此集合的元素复制到指定数组中，从指定的数组索引开始。 |
| [GetEnumerator](../../aspose.tasks/tablefieldcollection/getenumerator/)() | 返回此集合的枚举器。 |
| [IndexOf](../../aspose.tasks/tablefieldcollection/indexof/)(TableField) | 确定此集合中指定项的索引。 |
| [Insert](../../aspose.tasks/tablefieldcollection/insert/)(int, TableField) | 在指定索引处插入指定项。 |
| [Remove](../../aspose.tasks/tablefieldcollection/remove/)(TableField) | 从此集合中移除特定对象的第一次出现。 |
| [RemoveAt](../../aspose.tasks/tablefieldcollection/removeat/)(int) | 在指定索引处移除一项。 |

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

* class [TableField](../tablefield/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


