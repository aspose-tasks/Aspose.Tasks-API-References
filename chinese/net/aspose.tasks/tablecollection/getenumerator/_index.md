---
title: "TableCollection.GetEnumerator"
second_title: "Aspose.Tasks for .NET API 参考"
description: "TableCollection 方法。 返回此集合的枚举器。"
type: docs
weight: 70
url: /zh/net/aspose.tasks/tablecollection/getenumerator/
---
## TableCollection.GetEnumerator method

返回此集合的枚举器。

```csharp
public IEnumerator<Table> GetEnumerator()
```

### 返回值

此集合的枚举器。

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


