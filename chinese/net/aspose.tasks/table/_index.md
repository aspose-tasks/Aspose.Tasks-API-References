---
title: "类 Table"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.Table 类。表示 Project 中的表格"
type: docs
weight: 2320
url: /zh/net/aspose.tasks/table/
---
## Table class

表示 Project 中的表。

```csharp
public class Table
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [Table](table/)() | 初始化 `Table` 类的新实例。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [AdjustHeaderRowHeight](../../aspose.tasks/table/adjustheaderrowheight/) { get; set; } | 获取或设置一个值，指示是否可以调整表格标题行的高度。 |
| [DateFormat](../../aspose.tasks/table/dateformat/) { get; set; } | 获取或设置表格的日期格式。 |
| [LockFirstColumn](../../aspose.tasks/table/lockfirstcolumn/) { get; set; } | 获取或设置一个值，指示表格的第一列是锁定还是可编辑。 |
| [Name](../../aspose.tasks/table/name/) { get; set; } | 获取或设置 Table 对象的名称。 |
| [RowHeight](../../aspose.tasks/table/rowheight/) { get; set; } | 获取或设置表格中的行高，行高以文本行数表示。 |
| [ShowAddNewColumn](../../aspose.tasks/table/showaddnewcolumn/) { get; set; } | 获取或设置一个值，指示是否显示“添加新列”界面。支持 MSP 2010 及更高版本。 |
| [ShowInMenu](../../aspose.tasks/table/showinmenu/) { get; set; } | 获取或设置一个值，指示项目是否在功能区“视图”选项卡的 Tables 下拉列表中显示表格名称。 |
| [TableFields](../../aspose.tasks/table/tablefields/) { get; } | 获取表示表格字段的 TableFields 集合。 |
| [TableType](../../aspose.tasks/table/tabletype/) { get; set; } | 获取或设置指定表格的表格类型。 |
| [Uid](../../aspose.tasks/table/uid/) { get; } | 获取表的唯一标识符。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| override [Equals](../../aspose.tasks/table/equals/)(object) | 返回一个值，指示此实例是否等于指定的对象。 |
| override [GetHashCode](../../aspose.tasks/table/gethashcode/)() | 返回此表的哈希码。 |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


