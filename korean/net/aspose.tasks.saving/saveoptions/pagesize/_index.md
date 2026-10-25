---
title: "SaveOptions.PageSize"
second_title: "Aspose.Tasks for .NET API 참조"
description: "SaveOptions 속성. 렌더링될 페이지의 크기를 가져오거나 설정합니다. 기본값은 PageSize.A4입니다"
type: docs
weight: 130
url: /ko/net/aspose.tasks.saving/saveoptions/pagesize/
---
## SaveOptions.PageSize property

렌더링될 페이지 크기를 가져오거나 설정합니다 (기본값은 PageSize.A4).

```csharp
public PageSize PageSize { get; set; }
```

## 예제

페이지 크기를 설정하는 방법을 보여줍니다 ( &lt;see cref=\"P:Aspose.Tasks.Visualization.TiffCompression\" /&gt; 열거형의 값 중 하나일 수 있습니다).

```csharp
var project = new Project(DataDir + "Project2.mpp");

const PresentationFormat format = PresentationFormat.GanttChart;

// 프로젝트를 모든 사전 정의된 페이지 크기로 렌더링합니다
foreach (var pageSize in (PageSize[])Enum.GetValues(typeof(PageSize)))
{
    var options = new PdfSaveOptions
    {
        PresentationFormat = format,
        FitContent = true,
        PageSize = pageSize
    };
    project.Save(OutDir + "PredefinedPageSizes_" + format + "_" + pageSize + "_out.pdf", options);
}
```

### 또 보기

* enum [PageSize](../../../aspose.tasks.visualization/pagesize/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


