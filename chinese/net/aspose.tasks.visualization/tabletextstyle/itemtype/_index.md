---
title: "TableTextStyle.ItemType"
second_title: "Aspose.Tasks for .NET API 参考"
description: "TableTextStyle 属性。返回 TextItemType 枚举的值。"
type: docs
weight: 30
url: /zh/net/aspose.tasks.visualization/tabletextstyle/itemtype/
---
## TableTextStyle.ItemType property

返回 [`TextItemType`](../../textitemtype/) 枚举的值。

```csharp
public override TextItemType ItemType { get; }
```

## 示例

展示如何自定义表格文本样式，这些样式用于为项目中的不同文本项设置样式。

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Set(Prj.NewTasksAreManual, false);

var view = (GanttChartView)project.Views.ToList()[0];

// 设置第一个任务名称文本样式
var style1 = new TableTextStyle(1);
// 设置要应用样式的字段。
style1.Field = Field.TaskName;
// 设置文本样式的 <see cref=\"P:Aspose.Tasks.Visualization.TextStyle.Font\" />。
style1.Font = new FontDescriptor("Impact", 12F, FontStyles.Bold | FontStyles.Italic);
// 设置文本样式字体的点大小。

// 设置第二个任务持续时间文本样式
var style2 = new TableTextStyle(2);
style2.Field = Field.TaskDurationText;
style2.Font = new FontDescriptor("Impact", 16F, FontStyles.Underline);

view.TableTextStyles.Add(style1);
view.TableTextStyles.Add(style2);

SimpleSaveOptions options = new MPPSaveOptions
{
    // 设置指示必须写入视图数据的标志
    WriteViewData = true
};
project.Save(OutDir + "WorkWithTableTextStyle_out.mpp", options);
```

### 另见

* enum [TextItemType](../../textitemtype/)
* class [TableTextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../tabletextstyle/)
* assembly [Aspose.Tasks](../../../)


