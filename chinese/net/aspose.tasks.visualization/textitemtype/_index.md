---
title: "枚举 TextItemType"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.Visualization.TextItemType 枚举。用于更改文本样式的项目类型。"
type: docs
weight: 3410
url: /zh/net/aspose.tasks.visualization/textitemtype/
---
## TextItemType enumeration

用于更改文本样式的项目类型。

```csharp
public enum TextItemType
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| RowColumnTitles | `0` | 行和列标题。 |
| CriticalTasks | `1` | 关键任务。 |
| NoncriticalTasks | `2` | 非关键任务。 |
| MilestoneTasks | `3` | 里程碑任务。 |
| InactiveTasks | `4` | 非活动任务。 |
| SummaryTasks | `5` | 汇总任务。 |
| AssignmentRow | `6` | 分配行。 |
| TopTimescaleTier | `7` | 顶部时间尺度层。 |
| BottomTimescaleTier | `8` | 底部时间尺度层。 |
| MiddleTimescaleTier | `9` | 中部时间尺度层。 |
| Resources | `10` | 资源表。 |
| OverallocatedResources | `11` | 资源超额分配。 |
| TaskFilterHighlight | `12` | 任务过滤器高亮文本项。 |
| BarTextBottom | `13` | 条形文本底部文本项。 |
| BarTextInside | `14` | 条形文本内部文本项。 |
| BarTextLeft | `15` | 条形文本左侧文本项。 |
| BarTextRight | `16` | 条形文本右侧文本项。 |
| BarTextTop | `17` | 条形文本顶部文本项。 |
| MarkedTasks | `18` | 标记任务文本项。 |
| ProjectSummary | `19` | 项目汇总任务文本项。 |
| ExternalTasks | `20` | 外部任务文本项。 |
| Allocated | `21` | 已分配文本项。 |
| ChangedCells | `22` | 已更改的单元格。 |

## 示例

展示如何使用文本项类型。

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
SaveOptions options = new PdfSaveOptions
{
    PresentationFormat = PresentationFormat.ResourceSheet
};

var style = new TextStyle(FontStyles.Italic | FontStyles.Bold)
{
    Color = Color.OrangeRed
};

style.ItemType = TextItemType.OverallocatedResources;

options.TextStyles = new List<TextStyle>
{
    style
};
project.Save(OutDir + "CustomizeTextStyle_out.pdf", options);
```

### 另见

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


