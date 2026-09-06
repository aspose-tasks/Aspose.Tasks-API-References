---
title: "类 GanttBarStyle"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.Visualization.GanttBarStyle 类。表示 MSP 在甘特图视图中使用的条形样式"
type: docs
weight: 3070
url: /zh/net/aspose.tasks.visualization/ganttbarstyle/
---
## GanttBarStyle class

表示在甘特图视图中由 MSP 使用的条形样式。

```csharp
public class GanttBarStyle
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [GanttBarStyle](ganttbarstyle/)() | 初始化 `GanttBarStyle` 类的新实例。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [BottomBarTextConverter](../../aspose.tasks.visualization/ganttbarstyle/bottombartextconverter/) { get; set; } | 获取或设置用户定义的转换器，以获取在任务栏底部渲染的文本。覆盖 [`BottomField`](./bottomfield/) 属性的值。 |
| [BottomField](../../aspose.tasks.visualization/ganttbarstyle/bottomfield/) { get; set; } | 获取或设置显示在栏底部的数据。[`Field`](../../aspose.tasks/field/)。 |
| [EndShape](../../aspose.tasks.visualization/ganttbarstyle/endshape/) { get; set; } | 获取或设置栏的结束形状。 |
| [EndShapeColor](../../aspose.tasks.visualization/ganttbarstyle/endshapecolor/) { get; set; } | 获取或设置结束形状的颜色。 |
| [EndShapeType](../../aspose.tasks.visualization/ganttbarstyle/endshapetype/) { get; set; } | 获取或设置结束形状的类型。[`GanttBarType`](../ganttbartype/)。 |
| [From](../../aspose.tasks.visualization/ganttbarstyle/from/) { get; set; } | 获取或设置甘特栏的起始点位置。[`Field`](../../aspose.tasks/field/)。 |
| [InsideBarTextConverter](../../aspose.tasks.visualization/ganttbarstyle/insidebartextconverter/) { get; set; } | 获取或设置用户定义的转换器，以获取在任务栏内部渲染的文本。覆盖 [`InsideField`](./insidefield/) 属性的值。 |
| [InsideField](../../aspose.tasks.visualization/ganttbarstyle/insidefield/) { get; set; } | 获取或设置显示在栏内部的数据。[`Field`](../../aspose.tasks/field/)。 |
| [LeftBarTextConverter](../../aspose.tasks.visualization/ganttbarstyle/leftbartextconverter/) { get; set; } | 获取或设置用户定义的转换器，以获取在任务栏左侧渲染的文本。覆盖 [`LeftField`](./leftfield/) 属性的值。此设置不会持久化到 MPP 格式。 |
| [LeftField](../../aspose.tasks.visualization/ganttbarstyle/leftfield/) { get; set; } | 获取或设置显示在栏左侧的数据。[`Field`](../../aspose.tasks/field/)。 |
| [MiddleFillPattern](../../aspose.tasks.visualization/ganttbarstyle/middlefillpattern/) { get; set; } | 获取或设置甘特栏的填充图案。 |
| [MiddleShape](../../aspose.tasks.visualization/ganttbarstyle/middleshape/) { get; set; } | 获取或设置栏的中间形状。 |
| [MiddleShapeColor](../../aspose.tasks.visualization/ganttbarstyle/middleshapecolor/) { get; set; } | 获取或设置中间形状的颜色。 |
| [Name](../../aspose.tasks.visualization/ganttbarstyle/name/) { get; set; } | 获取或设置样式的名称。 |
| [ParentStyle](../../aspose.tasks.visualization/ganttbarstyle/parentstyle/) { get; set; } | 获取或设置自定义任务特定样式的父（或通用）样式。 |
| [RightBarTextConverter](../../aspose.tasks.visualization/ganttbarstyle/rightbartextconverter/) { get; set; } | 获取或设置用户定义的转换器，以获取在任务栏右侧渲染的文本。覆盖 [`RightField`](./rightfield/) 属性的值。 |
| [RightField](../../aspose.tasks.visualization/ganttbarstyle/rightfield/) { get; set; } | 获取或设置显示在栏右侧的数据。[`Field`](../../aspose.tasks/field/)。 |
| [Row](../../aspose.tasks.visualization/ganttbarstyle/row/) { get; set; } | 获取或设置行号。范围可以是 1 到 4（默认值为 1）。 |
| [ShowForCategories](../../aspose.tasks.visualization/ganttbarstyle/showforcategories/) { get; set; } | 获取或设置样式适用的任务类别。适用于甘特图中栏的父（或通用）样式（参见 [`BarStyles`](../../aspose.tasks/ganttchartview/barstyles/)）。 |
| [ShowForTaskUid](../../aspose.tasks.visualization/ganttbarstyle/showfortaskuid/) { get; set; } | 获取或设置样式适用的任务的唯一标识。适用于甘特图中栏的任务特定样式（参见 [`CustomBarStyles`](../../aspose.tasks/ganttchartview/custombarstyles/)）。 |
| [StartShape](../../aspose.tasks.visualization/ganttbarstyle/startshape/) { get; set; } | 获取或设置栏的起始形状。 |
| [StartShapeColor](../../aspose.tasks.visualization/ganttbarstyle/startshapecolor/) { get; set; } | 获取或设置起始形状的颜色。 |
| [StartShapeType](../../aspose.tasks.visualization/ganttbarstyle/startshapetype/) { get; set; } | 获取或设置起始形状的类型。 |
| [To](../../aspose.tasks.visualization/ganttbarstyle/to/) { get; set; } | 获取或设置甘特栏的结束点位置。 |
| [TopBarTextConverter](../../aspose.tasks.visualization/ganttbarstyle/topbartextconverter/) { get; set; } | 获取或设置用户定义的转换器，以获取在任务栏顶部渲染的文本。覆盖 [`TopField`](./topfield/) 属性的值。 |
| [TopField](../../aspose.tasks.visualization/ganttbarstyle/topfield/) { get; set; } | 获取或设置显示在栏顶部的数据。 |

## 示例

展示如何使用甘特图视图的自定义条样式。

```csharp
var project = new Project(DataDir + "Project2.mpp");

var ganttChartView = (GanttChartView)project.Views.First(v => v.Name == "Gantt &Chart");
PdfSaveOptions saveOptions = new PdfSaveOptions();
saveOptions.Timescale = Timescale.DefinedInView;
saveOptions.ViewSettings = ganttChartView;

// 条样式可以是任务特定的（位于 GanttChartView.CustomBarStyles）
// 或类别特定的（位于 GanttChartView.BarStyles）
foreach (GanttBarStyle ganttBarStyle in ganttChartView.CustomBarStyles)
{
    if (ganttBarStyle.ShowForTaskUid != 4)
    {
        continue;
    }

    // 出于演示目的，我们正在修改唯一 ID 为 4 的任务的样式
    // 这里我们将字段 (TaskName) 设置为在任务条的左侧渲染。
    ganttBarStyle.LeftField = Field.TaskName;
    // 这里我们设置自定义转换器，以控制应在任务条内部渲染的文本。
    ganttBarStyle.InsideBarTextConverter = task => "Hours rem.: " + (int)task.Get(Tsk.RemainingWork).TimeSpan.TotalHours;

    ganttBarStyle.MiddleShapeColor = Color.Green;
    ganttBarStyle.MiddleShape = GanttBarMiddleShape.LineTop;
    ganttBarStyle.StartShape = GanttBarEndShape.LeftBracket;
    ganttBarStyle.StartShapeColor = Color.Aqua;
    ganttBarStyle.EndShape = GanttBarEndShape.RightBracket;
    ganttBarStyle.EndShapeColor = Color.Aquamarine;
}

foreach (GanttBarStyle ganttBarStyle in ganttChartView.BarStyles)
{
    if (!ganttBarStyle.ShowForCategories.Contains(GanttBarShowFor.Milestone))
    {
        continue;
    }

    // 出于演示目的，我们正在修改适用于里程碑任务的样式。

    ganttBarStyle.StartShape = GanttBarEndShape.Diamond;
    ganttBarStyle.RightField = Field.TaskActualFinish;
    ganttBarStyle.TopBarTextConverter = task => task.Get(Tsk.ActualStart).Day.ToString();
}

project.Save(OutDir + "WorkWithGanttChartViewBarStyles_out.pdf", saveOptions);
```

展示如何读取视图的自定义栏样式。

```csharp
var project = new Project(DataDir + "CustomBarStyle.mpp");

var view = (GanttChartView)project.DefaultView;
Console.WriteLine("Custom bar styles count: {0}", view.CustomBarStyles.Count);

var style1 = view.CustomBarStyles[0];
Console.WriteLine("Style1.ParentStyle Name: {0}", style1.ParentStyle.Name);
Console.WriteLine("Style1.LeftField: {0}", style1.LeftField);
Console.WriteLine("Style1.RightField: {0}", style1.RightField);
Console.WriteLine("Style1.TopField: {0}", style1.TopField);
Console.WriteLine("Style1.BottomField: {0}", style1.BottomField);
Console.WriteLine("Style1.InsideField: {0}", style1.InsideField);
Console.WriteLine("Style1.From: {0}", style1.From);
Console.WriteLine("Style1.To: {0}", style1.To);
Console.WriteLine("Style1.Row: {0}", style1.Row);

var style2 = view.CustomBarStyles[1];
Console.WriteLine("Style2.LeftField: {0}", style2.LeftField);
Console.WriteLine("Style2.RightField: {0}", style2.RightField);
Console.WriteLine("Style2.TopField: {0}", style2.TopField);
Console.WriteLine("Style2.BottomField: {0}", style2.BottomField);
Console.WriteLine("Style2.InsideField: {0}", style2.InsideField);
Console.WriteLine("Style2.From: {0}", style2.From);
Console.WriteLine("Style2.To: {0}", style2.To);
Console.WriteLine("Style2.Row: {0}", style1.Row);

var style3 = view.CustomBarStyles[2];
Console.WriteLine("Style3.LeftField: {0}", style3.LeftField);
Console.WriteLine("Style3.RightField: {0}", style3.RightField);
Console.WriteLine("Style3.TopField: {0}", style3.TopField);
Console.WriteLine("Style3.BottomField: {0}", style3.BottomField);
Console.WriteLine("Style3.InsideField: {0}", style3.InsideField);

Console.WriteLine("Style3.StartShape: {0}", style3.StartShape);
Console.WriteLine("Style3.StartShapeType: {0}", style3.StartShapeType);
Console.WriteLine("Style3.StartShapeColor: {0}", style3.StartShapeColor);

Console.WriteLine("Style3.EndShape: {0}", style3.EndShape);
Console.WriteLine("Style3.EndShapeType: {0}", style3.EndShapeType);
Console.WriteLine("Style3.EndShapeColor: {0}", style3.EndShapeColor);

Console.WriteLine("Style3.MiddleShape: {0}", style3.MiddleShape);
Console.WriteLine("Style3.MiddleFillPattern: {0}", style3.MiddleFillPattern);
Console.WriteLine("Style3.MiddleShapeColor: {0}", style3.MiddleShapeColor);
Console.WriteLine("Style3.From: {0}", style3.From);
Console.WriteLine("Style3.To: {0}", style3.To);
Console.WriteLine("Style3.Row: {0}", style1.Row);
```

### 另见

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


