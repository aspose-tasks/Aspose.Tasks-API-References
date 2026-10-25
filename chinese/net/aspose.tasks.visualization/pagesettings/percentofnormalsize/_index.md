---
title: "PageSettings.PercentOfNormalSize"
second_title: "Aspose.Tasks for .NET API 参考"
description: "PageSettings 属性。获取或设置用于调整打印的正常尺寸的百分比"
type: docs
weight: 90
url: /zh/net/aspose.tasks.visualization/pagesettings/percentofnormalsize/
---
## PageSettings.PercentOfNormalSize property

获取或设置用于调整打印的正常大小的百分比。

```csharp
public int PercentOfNormalSize { get; set; }
```

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


