---
title: "Project.Tables"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Project 属性。获取 Table 对象的列表"
type: docs
weight: 900
url: /zh/net/aspose.tasks/project/tables/
---
## Project.Tables property

获取 [`Table`](../../table/) 对象的列表。

```csharp
public TableCollection Tables { get; }
```

## 示例

展示如何配置 Gantt Chart 属性。

```csharp
var project = new Project(DataDir + "Project5.mpp");
    var task = project.RootTask.Children.Add("New Activity");

    // 定义新的自定义属性
    var definition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Text1, null);
    project.ExtendedAttributes.Add(definition);

    // 向已创建的任务添加自定义文本属性。
    task.ExtendedAttributes.Add(definition.CreateExtendedAttribute("Activity attribute"));

    // 通过添加文本属性字段来自定义表格
    var field = new TableField
    {
        Field = Field.TaskText1,
        Width = 20,
        Title = "Custom attribute",
        AlignTitle = HorizontalStringAlignment.Center,
        AlignData = HorizontalStringAlignment.Center
    };

    var table = project.Tables.ToList()[0];
    table.TableFields.Insert(3, field);

    project.Save(OutDir + @"ConfigureGantChart_out.mpp", new MPPSaveOptions { WriteViewData = true });
}
catch (NotSupportedException ex)
{
    Console.WriteLine(
        ex.Message
        + "\nThis example will only work if you apply a valid Aspose License. You can purchase full license or get 30 day temporary license from http:// Www.aspose.com/purchase/default.aspx.");
}
```

### 另见

* class [TableCollection](../../tablecollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


