---
title: "Table.TableFields"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Table 属性。获取表示表中字段的 TableFields 集合"
type: docs
weight: 90
url: /zh/net/aspose.tasks/table/tablefields/
---
## Table.TableFields property

获取表示表格字段的 TableFields 集合。

```csharp
public TableFieldCollection TableFields { get; }
```

## 示例

展示如何使用项目的表格。

```csharp
var project = new Project(DataDir + "Project5.mpp");
var task = project.RootTask.Children.Add("New Activity");

// 定义新的自定义属性
var definition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Text1, null);
project.ExtendedAttributes.Add(definition);

// 向已创建的任务添加自定义文本属性。
task.ExtendedAttributes.Add(definition.CreateExtendedAttribute("Activity attribute"));

// 通过添加文本属性字段来自定义表格
var field = new TableField();
field.Field = Field.TaskText1;
field.Width = 20;
field.Title = "Custom attribute";
field.AlignTitle = HorizontalStringAlignment.Center;
field.AlignData = HorizontalStringAlignment.Center;

var table = project.Tables.ToList()[0];
table.TableFields.Insert(3, field);

project.Save(OutDir + "ConfigureGanttChart_out.mpp", new MPPSaveOptions { WriteViewData = true });
```

### 另见

* class [TableFieldCollection](../../tablefieldcollection/)
* class [Table](../)
* namespace [Aspose.Tasks](../../table/)
* assembly [Aspose.Tasks](../../../)


