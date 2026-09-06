---
title: "Table.Uid"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Table 属性。获取表的唯一标识符"
type: docs
weight: 110
url: /zh/net/aspose.tasks/table/uid/
---
## Table.Uid property

获取表的唯一标识符。

```csharp
public int Uid { get; }
```

## 示例

展示如何定义新表（用于视图）。

```csharp
var project = new Project(DataDir + "Project1.mpp");

// 获取要编辑的表
var table = project.Tables.ToList()[0];
Console.WriteLine("Uid of the table: " + table.Uid);
Console.WriteLine("Name of the table: " + table.Name);
Console.WriteLine("Type of the table: " + table.TableType);

// 调整一些属性
// 设置一个值，指示表的标题行高度是否可以调整
table.AdjustHeaderRowHeight = true;

// 设置表的日期格式。
table.DateFormat = DateFormat.DateDdMmYyyy;

// 设置一个值，指示表的第一列是锁定还是可编辑
table.LockFirstColumn = true;

// 设置表中的行高，行高以文本行数表示
table.RowHeight = 10;

// 设置一个值，指示是否显示“添加新列”界面
table.ShowAddNewColumn = true;

// 设置一个值，指示项目是否在功能区“视图”选项卡的“表”下拉列表中显示表名
table.ShowInMenu = true;

// 保存已更新的表
project.Save(OutDir + "WorkWithTable_out.mpp", SaveFileFormat.Mpp);
```

### 另见

* class [Table](../)
* namespace [Aspose.Tasks](../../table/)
* assembly [Aspose.Tasks](../../../)


