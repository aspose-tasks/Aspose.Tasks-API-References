---
title: "类 TableCollection"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.TableCollection 类。包含 Table 对象的列表。实现 ICollectionTable 接口"
type: docs
weight: 2330
url: /zh/net/aspose.tasks/tablecollection/
---
## TableCollection class

包含 [`Table`](../table/) 对象的列表。实现 ICollection&lt;Table&gt; 接口。

```csharp
public class TableCollection : ICollection<Table>
```

## 属性

| 名称 | 描述 |
| --- | --- |
| [Count](../../aspose.tasks/tablecollection/count/) { get; } | 获取此集合中包含的元素数量。 |
| [IsReadOnly](../../aspose.tasks/tablecollection/isreadonly/) { get; } | 获取一个值，指示此集合是否为只读；否则为 false。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| [Add](../../aspose.tasks/tablecollection/add/)(Table) | 将指定项添加到此集合中。 |
| [Clear](../../aspose.tasks/tablecollection/clear/)() | 从此集合中移除所有项。 |
| [Contains](../../aspose.tasks/tablecollection/contains/)(Table) | 如果在此集合中找到指定项则返回 true；否则返回 false。 |
| [CopyTo](../../aspose.tasks/tablecollection/copyto/)(Table[], int) | 将此集合的元素复制到指定数组中，从指定的数组索引开始。 |
| [GetEnumerator](../../aspose.tasks/tablecollection/getenumerator/)() | 返回此集合的枚举器。 |
| [Remove](../../aspose.tasks/tablecollection/remove/)(Table) | 从此集合中移除特定对象的第一次出现。 |
| [ToList](../../aspose.tasks/tablecollection/tolist/)() | 将表集合转换为 [`Table`](../table/) 对象的列表。 |

## 示例

展示如何使用表集合。

```csharp
var project = new Project(DataDir + "Project1.mpp");

Console.WriteLine("Is collection of tables read-only?: " + project.Tables.IsReadOnly);

// 遍历表格
Console.WriteLine("Print tables of " + project.Get(Prj.Name) + " project.");
Console.WriteLine("Table count: " + project.Tables.Count);
foreach (var tbl in project.Tables)
{
    Console.WriteLine("Name: " + tbl.Name);

    Console.WriteLine("Fields:");

    foreach (var field in tbl.TableFields)
    {
        Console.WriteLine("    {0} - '{1}' - {2}", field.Field, field.Title, field.Width);
    }
}

// 添加新表
var tableToAdd = new Table
{
    Name = "New Table",
    ShowInMenu = true
};
project.Tables.Add(tableToAdd);

Console.WriteLine("The collection contains the new table?: " + project.Tables.Contains(tableToAdd));

// 可以通过两种方式清除集合
if (deleteOneByOne)
{
    // 将表复制到数组中并逐个删除
    var tables = new Table[project.Tables.Count];
    project.Tables.CopyTo(tables, 0);
    foreach (var table in tables)
    {
        project.Tables.Remove(table);
    }
}
else
{
    // 或者可以完全清除表集合
    project.Tables.Clear();
}

// 该集合可以转换为普通的表列表
List<Table> list = project.Tables.ToList();
foreach (var table in list)
{
    Console.WriteLine("Name: " + table.Name);
}
```

### 另见

* class [Table](../table/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


