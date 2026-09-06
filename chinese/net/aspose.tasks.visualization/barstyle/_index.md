---
title: "类 BarStyle"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.Visualization.BarStyle 类。更改项目视图中项目条形的视觉样式"
type: docs
weight: 2960
url: /zh/net/aspose.tasks.visualization/barstyle/
---
## BarStyle class

更改项目视图中项目条形的视觉样式。

```csharp
public class BarStyle
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [BarStyle](barstyle/)() | 初始化 `BarStyle` 类的新实例。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [BarColor](../../aspose.tasks.visualization/barstyle/barcolor/) { get; set; } | 获取或设置条形样式的颜色。 |
| [BarShape](../../aspose.tasks.visualization/barstyle/barshape/) { get; set; } | 获取或设置条形样式的 [`BarShape`](./barshape/)。 |
| [BottomBarTextConverter](../../aspose.tasks.visualization/barstyle/bottombartextconverter/) { get; set; } | 获取或设置用户定义的转换器，以获取在任务栏底部渲染的文本。覆盖 [`BottomField`](./bottomfield/) 属性的值。 |
| [BottomField](../../aspose.tasks.visualization/barstyle/bottomfield/) { get; set; } | 获取或设置显示在条形底部的字段。 |
| [EndShape](../../aspose.tasks.visualization/barstyle/endshape/) { get; set; } | 获取或设置条形末端的 [`Shape`](../shape/)。 |
| [EndShapeColor](../../aspose.tasks.visualization/barstyle/endshapecolor/) { get; set; } | 获取或设置条形末端形状的颜色。 |
| [EndShapeType](../../aspose.tasks.visualization/barstyle/endshapetype/) { get; set; } | 获取或设置结束形状的类型。[`GanttBarType`](../ganttbartype/)。 |
| [From](../../aspose.tasks.visualization/barstyle/from/) { get; set; } | 获取或设置甘特栏的起始点位置。[`Field`](../../aspose.tasks/field/)。 |
| [InsideBarTextConverter](../../aspose.tasks.visualization/barstyle/insidebartextconverter/) { get; set; } | 获取或设置用户定义的转换器，以获取在任务栏内部渲染的文本。覆盖 [`InsideField`](./insidefield/) 属性的值。 |
| [InsideField](../../aspose.tasks.visualization/barstyle/insidefield/) { get; set; } | 获取或设置显示在条形内部的字段。 |
| [ItemType](../../aspose.tasks.visualization/barstyle/itemtype/) { get; set; } | 获取或设置条形样式的 [`BarItemType`](../baritemtype/)。 |
| [LeftBarTextConverter](../../aspose.tasks.visualization/barstyle/leftbartextconverter/) { get; set; } | 获取或设置用户定义的转换器，以获取在任务条形左侧渲染的文本。覆盖 [`LeftField`](./leftfield/) 属性的值。 |
| [LeftField](../../aspose.tasks.visualization/barstyle/leftfield/) { get; set; } | 获取或设置显示在条形左侧的字段。 |
| [RightBarTextConverter](../../aspose.tasks.visualization/barstyle/rightbartextconverter/) { get; set; } | 获取或设置用户定义的转换器，以获取在任务栏右侧渲染的文本。覆盖 [`RightField`](./rightfield/) 属性的值。 |
| [RightField](../../aspose.tasks.visualization/barstyle/rightfield/) { get; set; } | 获取或设置在栏右侧显示的字段。 |
| [StartShape](../../aspose.tasks.visualization/barstyle/startshape/) { get; set; } | 获取或设置栏起始处的[`Shape`](../shape/)。 |
| [StartShapeColor](../../aspose.tasks.visualization/barstyle/startshapecolor/) { get; set; } | 获取或设置栏起始处形状的颜色。 |
| [StartShapeType](../../aspose.tasks.visualization/barstyle/startshapetype/) { get; set; } | 获取或设置起始形状的类型。 |
| [TextStyle](../../aspose.tasks.visualization/barstyle/textstyle/) { get; set; } | 获取或设置栏文本的样式。 |
| [To](../../aspose.tasks.visualization/barstyle/to/) { get; set; } | 获取或设置甘特栏的结束点位置。 |
| [TopBarTextConverter](../../aspose.tasks.visualization/barstyle/topbartextconverter/) { get; set; } | 获取或设置用户定义的转换器，以获取在任务栏顶部渲染的文本。覆盖 [`TopField`](./topfield/) 属性的值。 |
| [TopField](../../aspose.tasks.visualization/barstyle/topfield/) { get; set; } | 获取或设置显示在栏顶部的字段。 |

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


