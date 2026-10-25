---
title: "PageSettings.AdjustToPercentOfNormalSize"
second_title: "Aspose.Tasks for .NET API 参考"
description: "PageSettings 属性。获取或设置一个值，指示是否将打印调整为指定的正常尺寸百分比 PercentOfNormalSize"
type: docs
weight: 20
url: /zh/net/aspose.tasks.visualization/pagesettings/adjusttopercentofnormalsize/
---
## PageSettings.AdjustToPercentOfNormalSize property

获取或设置一个值，指示是否将打印调整为指定的正常尺寸百分比（[`PercentOfNormalSize`](../percentofnormalsize/)）。

```csharp
public bool AdjustToPercentOfNormalSize { get; set; }
```

## 备注

在项目以 HTML 格式渲染时无效。

## 示例

展示如何使用指定的比例因子渲染视图。

```csharp
var project = new Project(DataDir + "Input.mpp");

var view = project.Views.First(v => v.Screen == ViewScreen.Gantt);

// 设置一个值，指示视图应使用指定的比例因子进行缩放
view.PageInfo.PageSettings.AdjustToPercentOfNormalSize = true;
// 指定比例因子
view.PageInfo.PageSettings.PercentOfNormalSize = 33;

PdfSaveOptions saveOptions = new PdfSaveOptions()
{
    ViewSettings = view,
    Timescale = Timescale.DefinedInView
};

project.Save(OutDir + "PrintViewWithSpecifiedScaleFactor_out.pdf", saveOptions);
```

### 另见

* class [PageSettings](../)
* namespace [Aspose.Tasks.Visualization](../../pagesettings/)
* assembly [Aspose.Tasks](../../../)


