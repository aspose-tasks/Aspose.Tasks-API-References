---
title: "SaveOptions.PageCount"
second_title: "Aspose.Tasks for .NET API 참조"
description: "SaveOptions 속성. 프로젝트의 페이지 수를 가져오거나 설정합니다."
type: docs
weight: 120
url: /ko/net/aspose.tasks.saving/saveoptions/pagecount/
---
## SaveOptions.PageCount property

프로젝트 페이지 수를 가져오거나 설정합니다.

```csharp
public int PageCount { get; }
```

## 예제

프로젝트의 선택된 페이지를 PDF 파일로 저장하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Software Development Plan.mpp");
var options = new PdfSaveOptions();
options.RenderToSinglePage = false;
options.Pages = new List<int>();

// 내보낼 수 있는 페이지 수를 확인해 봅시다
Console.WriteLine("Page Count: " + options.PageCount);

options.Pages.Add(1);
options.Pages.Add(4);
project.Save(OutDir + "SaveToMultiplePDFFiles_out.pdf", options);
```

### 또 보기

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


