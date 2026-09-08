---
title: "HtmlSaveOptions.UseGradientBrush"
second_title: "Aspose.Tasks for .NET API 참조"
description: "HtmlSaveOptions 속성. 프로젝트 레이아웃을 렌더링할 때 그라디언트 브러시를 사용할지 여부를 나타내는 값을 가져오거나 설정합니다. 현재 HTML로 렌더링할 때 그라디언트 브러시 사용은 지원되지 않습니다."
type: docs
weight: 160
url: /ko/net/aspose.tasks.saving/htmlsaveoptions/usegradientbrush/
---
## HtmlSaveOptions.UseGradientBrush property

프로젝트 레이아웃을 렌더링할 때 그라디언트 브러시를 사용할지 여부를 나타내는 값을 가져오거나 설정합니다. 현재 HTML로 렌더링할 때 그라디언트 브러시 사용은 지원되지 않습니다.

```csharp
public override bool UseGradientBrush { get; set; }
```

## 예제

프로젝트를 HTML 파일로 내보낼 때 사용할 사용자 정의 글꼴을 설정하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new HtmlSaveOptions
                  {
                      PresentationFormat = PresentationFormat.GanttChart,
                      FitContent = true
                  };

options.FontSettings.UseProjectDefaultFont = false;
options.FontSettings.DefaultFontName = "Segoe UI Black";
project.Save(OutDir + "AddDefaultFontDuringSavingAsHtml_out.html", options);
```

### 또 보기

* class [HtmlSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../htmlsaveoptions/)
* assembly [Aspose.Tasks](../../../)


