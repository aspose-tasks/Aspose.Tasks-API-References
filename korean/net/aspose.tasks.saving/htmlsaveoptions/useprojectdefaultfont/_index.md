---
title: "UseProjectDefaultFont"
second_title: "Aspose.Tasks for .NET API 참조"
description: "렌더링에 기본 글꼴을 사용해야 하는지 여부를 나타내는 값을 가져오거나 설정합니다."
type: docs
weight: 180
url: /ko/net/aspose.tasks.saving/htmlsaveoptions/useprojectdefaultfont/
---
## HtmlSaveOptions.UseProjectDefaultFont property

렌더링에 기본 글꼴을 사용해야 하는지 여부를 나타내는 값을 가져오거나 설정합니다.

```csharp
public bool UseProjectDefaultFont { get; set; }
```

### 비고

값이 False이고 DefaultFontName이 지정된 경우, 렌더링 엔진은 DefaultFontName에 지정된 글꼴을 대체 글꼴로 사용합니다. 그렇지 않으면 'Arial'(설치된 경우) 또는 'Generic Sans Serif' 글꼴이 대체 글꼴로 사용됩니다. 대체 글꼴은 현재 운영 체제에 설치되지 않은 글꼴을 텍스트 스타일이 참조할 때 프로젝트 뷰를 렌더링하는 동안 사용됩니다. 글꼴 해석을 보다 세밀하게 제어하려면 [`FontResolveCallback`](../fontresolvecallback) 콜백을 사용할 수 있습니다.

### 예제

프로젝트를 HTML 파일로 내보낼 때 사용할 사용자 정의 글꼴을 설정하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new HtmlSaveOptions
                  {
                      PresentationFormat = PresentationFormat.GanttChart,
                      FitContent = true,
                      UseProjectDefaultFont = false,
                      DefaultFontName = "Segoe UI Black"
                  };
project.Save(OutDir + "AddDefaultFontDuringSavingAsHtml_out.html", options);
```

### 또 보기

* class [HtmlSaveOptions](../../htmlsaveoptions)
* namespace [Aspose.Tasks.Saving](../../htmlsaveoptions)
* assembly [Aspose.Tasks](../../../)

<!-- 편집 금지: xmldocmd에 의해 Aspose.Tasks.dll용으로 생성됨 -->
