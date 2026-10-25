---
title: "DefaultFontName"
second_title: "Aspose.Tasks for .NET API 참조"
description: "렌더링을 위한 기본 또는 대체 글꼴을 가져오거나 설정합니다."
type: docs
weight: 40
url: /ko/net/aspose.tasks.saving/htmlsaveoptions/defaultfontname/
---
## HtmlSaveOptions.DefaultFontName property

렌더링에 사용할 기본(또는 대체) 글꼴을 가져오거나 설정합니다.

```csharp
public string DefaultFontName { get; set; }
```

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
