---
title: "UseProjectDefaultFont"
second_title: "Aspose.Tasks for .NET API 참조"
description: "렌더링에 기본 글꼴을 사용해야 하는지 여부를 나타내는 값을 가져오거나 설정합니다."
type: docs
weight: 110
url: /ko/net/aspose.tasks.saving/imagesaveoptions/useprojectdefaultfont/
---
## ImageSaveOptions.UseProjectDefaultFont property

렌더링에 기본 글꼴을 사용해야 하는지 여부를 나타내는 값을 가져오거나 설정합니다.

```csharp
public bool UseProjectDefaultFont { get; set; }
```

### 비고

값이 False이고 DefaultFontName이 지정된 경우, 렌더링 엔진은 DefaultFontName에 지정된 글꼴을 대체 글꼴로 사용합니다. 그렇지 않으면 'Arial'(설치된 경우) 또는 'Generic Sans Serif' 글꼴이 대체 글꼴로 사용됩니다. 대체 글꼴은 현재 운영 체제에 설치되지 않은 글꼴을 텍스트 스타일이 참조할 때 프로젝트 뷰를 렌더링하는 동안 사용됩니다. 글꼴 해석을 보다 세밀하게 제어하려면 [`FontResolveCallback`](../fontresolvecallback) 콜백을 사용할 수 있습니다.

### 예제

레이아웃을 별도의 파일로 저장하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Homemoveplan.mpp");
var options = new ImageSaveOptions(SaveFileFormat.Png);
options.StartDate = project.Get(Prj.StartDate).AddDays(-3);
options.EndDate = project.Get(Prj.FinishDate);
options.MarkCriticalTasks = true;
options.DefaultFontName = "Segoe UI Black";
options.UseProjectDefaultFont = false;
options.PageSize = PageSize.Letter;

options.Gridlines = new List<Gridline>();

var gridline = new Gridline { GridlineType = GridlineType.GanttRow, Color = Color.CornflowerBlue, Pattern = LinePattern.Dashed };
options.Gridlines.Add(gridline);

project.Save(OutDir + "PrintProjectPagesToSeparateFiles1_out.png", options);

// 프로젝트 레이아웃을 별도의 파일로 저장합니다.
options.RenderToSinglePage = false;
project.Save(OutDir + "PrintProjectPagesToSeparateFiles2_out.png", options);
```

### 또 보기

* class [ImageSaveOptions](../../imagesaveoptions)
* namespace [Aspose.Tasks.Saving](../../imagesaveoptions)
* assembly [Aspose.Tasks](../../../)

<!-- 편집 금지: xmldocmd에 의해 Aspose.Tasks.dll용으로 생성됨 -->
