---
title: "FontSettings.FontResolveCallback"
second_title: "Aspose.Tasks for .NET API 참조"
description: "FontSettings 속성. 해결된 글꼴을 사용자 정의하는 데 사용할 수 있는 콜백을 가져오거나 설정합니다."
type: docs
weight: 30
url: /ko/net/aspose.tasks/fontsettings/fontresolvecallback/
---
## FontSettings.FontResolveCallback property

해결된 글꼴을 사용자 지정하는 데 사용할 수 있는 콜백을 가져오거나 설정합니다.

```csharp
public FontResolveCallbackDelegate FontResolveCallback { get; set; }
```

## 예제

대체 글꼴을 설정하거나 특정 글꼴을 교체하기 위해 사용자 정의 코드를 실행하는 사용자 지정 글꼴 해결 콜백을 설정하는 방법을 보여줍니다.

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
        // 정확한 글꼴을 찾을 수 없으며 대체 글꼴이 설정된 것으로 보입니다.
        // 대체 글꼴을 재정의할 수 있습니다.
        args.ResolvedFontName = "Arial";
    }

    // 또는 간단히 특정 글꼴을 교체합니다:
    if (args.RequestedFontName == "Comic Sans MS")
    {
        args.ResolvedFontName = "Arial";
    }
};

project.Save(OutDir + "EstimatedMilestoneTasks_out3.pdf", options);
```

### 또 보기

* delegate [FontResolveCallbackDelegate](../../fontresolvecallbackdelegate/)
* class [FontSettings](../)
* namespace [Aspose.Tasks](../../fontsettings/)
* assembly [Aspose.Tasks](../../../)


