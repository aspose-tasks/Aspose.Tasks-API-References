---
title: "PageSettings.PagesInWidth"
second_title: "Aspose.Tasks for .NET API 参考"
description: "PageSettings 属性。获取或设置要打印的宽度页数"
type: docs
weight: 60
url: /zh/net/aspose.tasks.visualization/pagesettings/pagesinwidth/
---
## PageSettings.PagesInWidth property

获取或设置要打印的水平页数。

```csharp
public int PagesInWidth { get; set; }
```

## 示例

展示如何使用 “Fit X to Y pages” 选项渲染视图。

```csharp
var project = new Project(DataDir + "TaskUsageView.mpp");

var view = project.Views.First(v => v.Screen == ViewScreen.TaskUsage);

view.PageInfo.PageSettings.AdjustToPercentOfNormalSize = false;
// 指定视图应在高度上渲染为 2 页或更少
view.PageInfo.PageSettings.PagesInHeight = 2;
// 指定视图应在宽度上渲染为 1 页
view.PageInfo.PageSettings.PagesInWidth = 1;

PdfSaveOptions saveOptions = new PdfSaveOptions()
{
    ViewSettings = view,
    Timescale = Timescale.DefinedInView,
    StartDate =  new DateTime(2000, 04, 1),
    EndDate = new DateTime(2000, 12, 31)
};

project.Save(OutDir + "PrintViewWithFitToPages_out.pdf", saveOptions);
```

### 另见

* class [PageSettings](../)
* namespace [Aspose.Tasks.Visualization](../../pagesettings/)
* assembly [Aspose.Tasks](../../../)


