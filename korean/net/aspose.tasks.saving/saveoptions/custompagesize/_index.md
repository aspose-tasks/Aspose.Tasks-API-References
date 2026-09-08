---
title: "SaveOptions.CustomPageSize"
second_title: "Aspose.Tasks for .NET API 참조"
description: "SaveOptions 속성. 포인트 단위(1 포인트 = 1/72 인치)의 사용자 정의 페이지 크기를 가져오거나 설정합니다."
type: docs
weight: 20
url: /ko/net/aspose.tasks.saving/saveoptions/custompagesize/
---
## SaveOptions.CustomPageSize property

맞춤 페이지 크기를 포인트 단위로 가져오거나 설정합니다 (1 포인트 = 1/72 인치).

```csharp
public SizeF CustomPageSize { get; set; }
```

## 예제

프로젝트를 PDF로 저장할 때 사용자 정의 페이지 크기를 설정하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions();
options.PresentationFormat = PresentationFormat.GanttChart;
options.CustomPageSize = new SizeF(5.8F * 72, 8.3F * 72);

project.Save(OutDir + "WorkWithCustomPageSize_out.pdf", options);
```

### 또 보기

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


