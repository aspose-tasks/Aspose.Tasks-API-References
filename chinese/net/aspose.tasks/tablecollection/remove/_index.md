---
title: "TableCollection.Remove"
second_title: "Aspose.Tasks for .NET API 参考"
description: "TableCollection 方法。 删除此集合中指定对象的第一次出现。"
type: docs
weight: 80
url: /zh/net/aspose.tasks/tablecollection/remove/
---
## TableCollection.Remove method

从此集合中移除特定对象的第一次出现。

```csharp
public bool Remove(Table item)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| item | Table | 要删除的指定对象。 |

### 返回值

如果成功从此集合中删除指定对象则返回 true；否则返回 false。

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

* class [Table](../../table/)
* class [TableCollection](../)
* namespace [Aspose.Tasks](../../tablecollection/)
* assembly [Aspose.Tasks](../../../)


