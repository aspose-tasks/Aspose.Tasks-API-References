---
title: "类 TableField"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.TableField 类。表示项目中表格的字段。"
type: docs
weight: 2340
url: /zh/net/aspose.tasks/tablefield/
---
## TableField class

表示项目中表的字段。

```csharp
public class TableField
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [TableField](tablefield/)() | 初始化 `TableField` 类的新实例。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [AlignData](../../aspose.tasks/tablefield/aligndata/) { get; set; } | 获取或设置表格字段中数据的对齐方式。 |
| [AlignTitle](../../aspose.tasks/tablefield/aligntitle/) { get; set; } | 获取或设置表格字段中标题的对齐方式。 |
| [Field](../../aspose.tasks/tablefield/field/) { get; set; } | 获取或设置表格字段的类型。 |
| [Title](../../aspose.tasks/tablefield/title/) { get; set; } | 获取或设置表格中字段的标题。 |
| [Width](../../aspose.tasks/tablefield/width/) { get; set; } | 获取或设置表格中字段列的宽度（以点为单位）。 |
| [WrapHeader](../../aspose.tasks/tablefield/wrapheader/) { get; set; } | 获取或设置一个值，指示表格列标题是否可以换行到多行，或者在超过列宽时是否应被截断。 |
| [WrapText](../../aspose.tasks/tablefield/wraptext/) { get; set; } | 获取或设置一个值，指示列文本是否可以换行到多行，或者在超过列宽时是否应被截断。支持 MSP 2010 版本及更高版本。 |

## 示例

展示如何使用 Project 的视图并向默认视图添加列（当在 MS Project 中打开 MPP 文件时显示的视图）。

```csharp
// 创建一个没有视图的空项目
var project = new Project();
project.Set(Prj.Name, "Test View Project");

// 修改默认视图（它是甘特图视图）。
// 或者您可以使用 project.View 集合通过名称或通过视图屏幕选择视图。
var view = (GanttChartView) project.DefaultView;

TableField newColumn = new TableField()
{
    AlignData = HorizontalStringAlignment.Center,
    Title = "My new column",
    Width = 30,
    Field = Field.TaskActualDuration
};

view.Table.TableFields.Add(newColumn);

// 应使用 WriteViewData 标志来持久化视图属性的修改。
project.Save(OutDir + "ModifyView_output.mpp", new Saving.MPPSaveOptions
{
    WriteViewData = true
});
```

展示如何读取项目表。

```csharp
var project = new Project(DataDir + "ReadTableData.mpp");

// 获取表
var table = project.Tables.ToList()[0];
Console.WriteLine("Print table fields of {0}", table.Name);
Console.WriteLine("Table Fields Count" + table.TableFields.Count);

// 显示所有表字段的信息
foreach (var field in table.TableFields)
{
    Console.WriteLine("  Field: " + field.Field);
    Console.WriteLine("  Width: " + field.Width);
    Console.WriteLine("  Title: " + field.Title);
    Console.WriteLine("  Title Alignment: " + field.AlignTitle);
    Console.WriteLine("  Data Alignment: " + field.AlignData);
    Console.WriteLine("  Wrap Header: " + field.WrapHeader);
    Console.WriteLine("  Wrap Text: " + field.WrapText);
    Console.WriteLine();
}
```

### 另见

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


