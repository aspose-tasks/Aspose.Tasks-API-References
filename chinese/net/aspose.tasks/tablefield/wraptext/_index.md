---
title: "TableField.WrapText"
second_title: "Aspose.Tasks for .NET API 参考"
description: "TableField 属性。获取或设置一个值，指示列文本是否可以换行到多行，或在超出列宽时是否应被截断。支持 MSP 2010 及更高版本"
type: docs
weight: 80
url: /zh/net/aspose.tasks/tablefield/wraptext/
---
## TableField.WrapText property

获取或设置一个值，指示列文本是否可以换行到多行，或者在超过列宽时是否应被截断。支持 MSP 2010 版本及更高版本。

```csharp
public bool WrapText { get; set; }
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

* class [TableField](../)
* namespace [Aspose.Tasks](../../tablefield/)
* assembly [Aspose.Tasks](../../../)


