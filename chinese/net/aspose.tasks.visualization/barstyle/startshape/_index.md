---
title: "BarStyle.StartShape"
second_title: "Aspose.Tasks for .NET API 参考"
description: "BarStyle 属性。获取或设置条形起始处的 Shape"
type: docs
weight: 170
url: /zh/net/aspose.tasks.visualization/barstyle/startshape/
---
## BarStyle.StartShape property

获取或设置[`Shape`](../../shape/)在条形起始处。

```csharp
public Shape StartShape { get; set; }
```

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

* enum [Shape](../../shape/)
* class [BarStyle](../)
* namespace [Aspose.Tasks.Visualization](../../barstyle/)
* assembly [Aspose.Tasks](../../../)


