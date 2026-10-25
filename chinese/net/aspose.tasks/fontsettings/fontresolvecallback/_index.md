---
title: "FontSettings.FontResolveCallback"
second_title: "Aspose.Tasks for .NET API 参考"
description: "FontSettings 属性。获取或设置可用于自定义已解析字体的回调函数"
type: docs
weight: 30
url: /zh/net/aspose.tasks/fontsettings/fontresolvecallback/
---
## FontSettings.FontResolveCallback property

获取或设置可用于自定义已解析字体的回调。

```csharp
public FontResolveCallbackDelegate FontResolveCallback { get; set; }
```

## 示例

展示如何设置自定义字体解析回调，以执行用户定义的代码来设置回退字体或替换特定字体。

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions
{
    PresentationFormat = PresentationFormat.GanttChart,
};

options.FontSettings.FontResolveCallback = delegate(FontResolveEventArgs args)
{
    if (args.RequestedFontName != args.ResolvedFontName)
    {
        // 看起来找不到确切的字体，已设置回退字体。
        // 我们可以覆盖回退字体。
        args.ResolvedFontName = "Arial";
    }

    // 或者直接替换特定字体：
    if (args.RequestedFontName == "Comic Sans MS")
    {
        args.ResolvedFontName = "Arial";
    }
};

project.Save(OutDir + "EstimatedMilestoneTasks_out3.pdf", options);
```

### 另见

* delegate [FontResolveCallbackDelegate](../../fontresolvecallbackdelegate/)
* class [FontSettings](../)
* namespace [Aspose.Tasks](../../fontsettings/)
* assembly [Aspose.Tasks](../../../)


