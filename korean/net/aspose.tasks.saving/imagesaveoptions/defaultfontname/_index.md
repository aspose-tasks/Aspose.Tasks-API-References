---
title: "DefaultFontName"
second_title: "Aspose.Tasks for .NET API 참조"
description: "렌더링을 위한 기본 또는 대체 글꼴을 가져오거나 설정합니다."
type: docs
weight: 20
url: /ko/net/aspose.tasks.saving/imagesaveoptions/defaultfontname/
---
## ImageSaveOptions.DefaultFontName property

렌더링에 사용할 기본(또는 대체) 글꼴을 가져오거나 설정합니다.

```csharp
public string DefaultFontName { get; set; }
```

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
