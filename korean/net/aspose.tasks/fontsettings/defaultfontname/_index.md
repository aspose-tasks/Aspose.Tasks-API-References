---
title: "FontSettings.DefaultFontName"
second_title: "Aspose.Tasks for .NET API 참조"
description: "FontSettings 속성. 렌더링을 위한 기본 또는 대체 글꼴을 가져오거나 설정합니다."
type: docs
weight: 20
url: /ko/net/aspose.tasks/fontsettings/defaultfontname/
---
## FontSettings.DefaultFontName property

렌더링에 사용할 기본(또는 대체) 글꼴을 가져오거나 설정합니다.

```csharp
public string DefaultFontName { get; set; }
```

## 예제

출력 PDF 인쇄에 사용할 사용자 지정 글꼴을 설정하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions
                  {
                      PresentationFormat = PresentationFormat.GanttChart, FitContent = true
                  };

options.FontSettings.UseProjectDefaultFont = false;
options.FontSettings.DefaultFontName = "Segoe UI Black";
project.Save(OutDir + "CreateProject2_out.pdf", options);
```

### 또 보기

* class [FontSettings](../)
* namespace [Aspose.Tasks](../../fontsettings/)
* assembly [Aspose.Tasks](../../../)


