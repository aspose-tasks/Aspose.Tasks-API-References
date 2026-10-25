---
title: "TableField.AlignData"
second_title: "Aspose.Tasks for .NET API 参考"
description: "TableField 属性。获取或设置表字段中数据的对齐方式"
type: docs
weight: 20
url: /zh/net/aspose.tasks/tablefield/aligndata/
---
## TableField.AlignData property

获取或设置表格字段中数据的对齐方式。

```csharp
public HorizontalStringAlignment AlignData { get; set; }
```

## 示例

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

* enum [HorizontalStringAlignment](../../../aspose.tasks.visualization/horizontalstringalignment/)
* class [TableField](../)
* namespace [Aspose.Tasks](../../tablefield/)
* assembly [Aspose.Tasks](../../../)


