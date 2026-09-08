---
title: "PdfSaveOptions.Pages"
second_title: "Aspose.Tasks for .NET API 참조"
description: "PdfSaveOptions 속성. 프로젝트 레이아웃을 별도의 파일로 저장할 때 저장할 페이지 번호 목록을 가져오거나 설정합니다. 이 목록이 비어 있으면 모든 페이지가 저장됩니다."
type: docs
weight: 60
url: /ko/net/aspose.tasks.saving/pdfsaveoptions/pages/
---
## PdfSaveOptions.Pages property

프로젝트 레이아웃을 별도 파일로 저장할 때 저장할 페이지 번호 목록을 가져오거나 설정합니다. 이 목록이 비어 있으면 모든 페이지가 저장됩니다.

```csharp
public List<int> Pages { get; set; }
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

* class [PdfSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../pdfsaveoptions/)
* assembly [Aspose.Tasks](../../../)


