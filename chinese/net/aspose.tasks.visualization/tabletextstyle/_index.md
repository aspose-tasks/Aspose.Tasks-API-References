---
title: "类 TableTextStyle"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.Visualization.TableTextStyle 类。表示视图表中的文本样式"
type: docs
weight: 3370
url: /zh/net/aspose.tasks.visualization/tabletextstyle/
---
## TableTextStyle class

表示视图表格中的文本样式。

```csharp
public class TableTextStyle : TextStyle
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [TableTextStyle](tabletextstyle/#constructor)(int) | 初始化 `TableTextStyle` 类的新实例。 |
| [TableTextStyle](tabletextstyle/#constructor_1)(int, FontDescriptor) | 使用指定的字体初始化 `TableTextStyle` 类的新实例。 |
| [TableTextStyle](tabletextstyle/#constructor_2)(int, FontStyles) | 使用默认字体设置和指定的字体样式初始化 `TableTextStyle` 类的新实例。 |
| [TableTextStyle](tabletextstyle/#constructor_3)(int, float, FontStyles) | 使用指定的字体大小和字体样式初始化 `TableTextStyle` 类的新实例。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [BackgroundColor](../../aspose.tasks.visualization/textstyle/backgroundcolor/) { get; set; } | 获取或设置文本样式的背景颜色。[`Color`](../textstyle/color/)。 |
| [BackgroundPattern](../../aspose.tasks.visualization/textstyle/backgroundpattern/) { get; set; } | 获取或设置文本样式的背景图案。[`BackgroundPattern`](../textstyle/backgroundpattern/)。 |
| [Color](../../aspose.tasks.visualization/textstyle/color/) { get; set; } | 获取或设置文本的颜色。 |
| [Field](../../aspose.tasks.visualization/tabletextstyle/field/) { get; set; } | 获取或设置样式要应用的字段。[`Field`](./field/)。 |
| [Font](../../aspose.tasks.visualization/textstyle/font/) { get; set; } | 获取或设置文本样式的字体。 |
| override [ItemType](../../aspose.tasks.visualization/tabletextstyle/itemtype/) { get; } | 返回 [`TextItemType`](../textitemtype/) 枚举的值。 |
| [RowUid](../../aspose.tasks.visualization/tabletextstyle/rowuid/) { get; } | 获取行的唯一 ID。如果样式要应用于视图的所有行，则返回 -1。 |

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

* class [TextStyle](../textstyle/)
* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


