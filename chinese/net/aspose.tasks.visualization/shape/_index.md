---
title: "枚举 Shape"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.Visualization.Shape 枚举。标记在条形样式的起始或结束处的形状，在将视图数据保存为某些 SaveFileFormat 时进行渲染。"
type: docs
weight: 3360
url: /zh/net/aspose.tasks.visualization/shape/
---
## Shape enumeration

在将视图数据保存为某些 [`SaveFileFormat`](../../aspose.tasks.saving/savefileformat/) 时，要渲染的条形样式起始或结束处的标记形状。

```csharp
public enum Shape
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| None | `0` | 指示无形状。 |
| VerticalLine | `1` | 指示垂直线形状。 |
| Pentagon | `2` | 指示五边形形状。 |
| Triangle | `3` | 指示三角形形状。 |
| LeftBracket | `4` | 指示左括号形状。 |
| RightBracket | `5` | 指示右括号形状。 |
| ArrowDown | `6` | 指示 ArrowDown 形状。 |
| LeftFade | `7` | 指示左淡化形状。 |
| RightFade | `8` | 指示右淡化形状。 |
| Diamond | `9` | 指示菱形形状。 |
| Circle | `10` | 指示圆形形状。 |

## 示例

展示如何使用自定义条形样式。

```csharp
var project = new Project(DataDir + "Project2.mpp");
SaveOptions options = new PdfSaveOptions
{
    BarStyles = new List<BarStyle>()
};

// 为里程碑任务添加条形样式
var style = new BarStyle();
// 设置条形样式的 <see cref=\"T:Aspose.Tasks.Visualization.BarItemType\" />
style.ItemType = BarItemType.Milestone;
// 设置条形样式的 <see cref=\"T:System.Drawing.Color\" />。
style.BarColor = Color.Green;
// 设置条形样式的 <see cref=\"P:Aspose.Tasks.Visualization.BarStyle.BarShape\" />
style.BarShape = BarShape.HalfHeight;
// 在条形的起始位置设置 <see cref=\"T:Aspose.Tasks.Visualization.Shape\" />
style.StartShape = Shape.LeftBracket;
// 在条形的起始位置设置形状的 <see cref=\"T:System.Drawing.Color\" />
style.StartShapeColor = Color.Aqua;
// 在条形的结束位置设置 <see cref=\"T:Aspose.Tasks.Visualization.Shape\" />
style.EndShape = Shape.RightBracket;
// 在条形的结束位置设置形状的 <see cref=\"T:System.Drawing.Color\" />
style.EndShapeColor = Color.Aquamarine;
// 设置在条形右侧渲染的文本。
style.TextStyle = new TextStyle();
style.TextStyle.BackgroundColor = Color.Black;

// 有一个功能可以将条形的文本转换。
// 让我们设置转换器来获取条形的渲染文本。
style.LeftBarTextConverter = task =>
{
    if (!task.Get(Tsk.Name).StartsWith("T"))
    {
        task.Set(Tsk.Name, "T" + task.Get(Tsk.Name));
    }

    return task.Get(Tsk.Name);
};

options.BarStyles.Add(style);

// 保存项目
project.Save(OutDir + "WorkWithBarStyle_out.mpp", options);
```

### 另见

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


