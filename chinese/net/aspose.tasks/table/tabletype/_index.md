---
title: "Table.TableType"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Table 属性。获取或设置指定表的表类型"
type: docs
weight: 100
url: /zh/net/aspose.tasks/table/tabletype/
---
## Table.TableType property

获取或设置指定表格的表格类型。

```csharp
public ItemType TableType { get; set; }
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

* enum [ItemType](../../itemtype/)
* class [Table](../)
* namespace [Aspose.Tasks](../../table/)
* assembly [Aspose.Tasks](../../../)


